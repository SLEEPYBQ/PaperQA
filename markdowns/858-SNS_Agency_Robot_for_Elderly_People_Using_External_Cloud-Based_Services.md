# SNS Agency Robot for Elderly People using External Cloud-based Services

Toru KOBAYASHI, Kazushige KATSURAGI, Taishi MIYAZAKI, and Kenichi ARAI Division of Electrical Engineering and Computer Science Graduate School of Engineering, Nagasaki University Nagasaki, Japan toru@cis.nagasaki-u.ac.jp

*Abstract***—We propose a SNS Agency Robot that can be used for the interactive communication between elderly people and younger generation via existing Social Networking Service (SNS). This robot system has been implemented on a cloud service and a single board computer embedded in a human-type robot, which is equipped with a microphone, camera, speaker, sensors, and network access function, so that elderly people can transmit and receive information by voice via SNS without using smartphones. We employed LINE that is a proprietary application for instant communications on electronic devices such as smartphones. In LINE, we need to select a message destination address before sending messages. On the other hand, our proposed robot is basically operated by voice due to realizing the simple user interface. Therefore, we proposed a message exchange learningtype destination estimation method that enables elderly people not to express a message destination address explicitly. We developed the prototype system including the message exchange learning-type destination estimation method. Then, we confirmed the effectiveness of the message destination estimation through the demonstration experiment at the house for the elderly with the care service.** 

*Keywords— SNS; Elderly people watching services; IoT; Service-oriented architecture; User interface; Robot* 

#### I. INTRODUCTION

Current state and trends on the elderly and their environment in Japan is really serious. According to this current situation, elderly people watching system has become important. However, most of the existing elderly people watching services are belonging to the service category of a confirmation of elderly people's safety based on one-way communication from elderly people [1][2][3]. Therefore, current services are not enough for elderly people who want to have more tight connection with society. On the other hand, SNS like Twitter has already become popular. However, people need to use smart devices like smartphones efficiently to access SNS. This matter might be obstacles for elderly people to use SNS. Therefore, we have proposed a Social Media Mediation System that can be used for the interactive communication between elderly people and younger generation via existing SNS like Twitter or Google Calendar [4][5]. We have implemented this proposed system on a single board computer embedded in a human-type robot, which is equipped with a microphone, camera, speaker, sensors and network

access function. Elderly people can transmit and receive information by voice via Twitter.

On the other hand, currently here in Japan, LINE has become a popular messaging service that we can exchange texts, images, video and audio, and conduct free VoIP conversations and video conferences [6]. LINE is also providing the Messaging API [7], so that we decide to employ LINE as SNS for our robot system. In LINE, we need to select a message destination address before sending messages. However, our proposed robot is basically operated only by voice due to realizing the simple user interface. Therefore, we proposed a message exchange learning-type destination estimation method that enables elderly people not to express a message destination address explicitly [8]. This method is based on the machine learning algorithm that performs the message destination estimation according to message contents of elderly people. We need a right message destination address as training data to increase the machine learning performance. However, if we asked elderly people to express a right message destination address to gather training data for machine learning, it would not make sense. Therefore, we designed the method that uses a response against a message from elderly people as training data. In this method, a message receiver's response against a message from elderly people would be applied to machine learning as training data, so that we could increase the machine learning performance without elderly people's effort.

We also re-designed the SNS Agency Robot based on the service-oriented architecture that enables us easily to use open innovation like external cloud-based services. For example, we used Google Cloud Speech API as speech recognition and IBM Watson Natural Language Classifier (NLC) as message destination estimation machine learning engine. We could expect that this feature allows us to launch a new communication system quickly at low cost. We developed the main functionality on Microsoft Azure as prototype system. In our previous work [4][5][8], the main functionality has been implemented on a single board computer embedded in a robot installed at elderly people's house, so that serviceability will be increased. We confirmed the effectiveness of the message destination estimation through the demonstration experiment. In order to evaluate the message destination estimation, we asked 3 subjects who are from 78 to 88 years old to use the prototype system at the house for the elderly with the care service at Togitsu-machi in Nagasaki prefecture in Japan.

0730-3157/17 \$31.00 © 2017 IEEE DOI 10.1109/COMPSAC.2017.216

![](_page_0_Picture_12.jpeg)

#### II. RELATED WORK

Recently, we can see many elderly people watching services or systems. For example, Zojirushi I-Pot [9], which is a water heater, can send an e-mail message to relatives when a single-living elderly person turns on the I-Pot in the morning. In this service, the relationship between elderly people and watchers is one-to-one. The information sending direction is one-way that is from elderly people to watchers. The existing relating services are focusing on a confirmation of elderly people's safety. Murase proposed the distance communication environment using activities in daily life like a setting action of an alarm clock as a trigger [10]. This research has been involved in the category of interactive and many-to-many communication. However, he implemented this system as an original communication application. Therefore, in order to use this system, watchers need to install the special application and learn how to use it.

On the other hand, we have some communication robot studies for elderly people. Inoue proposed a communication robot for elderly people and their families to support their daily lives [11]. He tried to analyze how families living with seniors feel about using the human-type communication robot. Sasama reported an experiment for motivating elderly people with robot-guided interaction [12]. He built a framework for encouraging elderly people to participate in more activities by providing local news. Kanoh executed an examination of practicability of communication robot-assisted activity program for elderly people [13]. He has developed a Robot Assisted Activity (RAA) program for recreational use in health care facilities for elderly people. These relating studies are focusing on encouraging elderly people to have more communication with closed people, so that remote communication functionality is not enough. We are focusing on the remote communication using SNS. This point is the different point.

We have also voice operation robots such as Amazon Echo [14], Google Home [15], and Pepper [16]. They are the robots with the artificial intelligence, so that people can operate them by voice to search information or control house appliances. However, we cannot communicate with the other persons via social media by using them. The different point is that our proposed robot enables us to communicate with the other persons via social media.

In terms of message filtering mechanism like Bayesian Filter, a spam filter for e-mail message is famous one [17] [18]. In this case, an e-mail receiver needs to decide whether received e-mail message would be spam e-mail or not. However, in our method, we use the response from people who get messages from elderly people, so that elderly people do not have to do anything for increasing machine learning performance. This point is completely different from a spam filter mechanism.

# III. USE CASE AND MESSAGE DESTINATION ESTIMATION

#### *A. Use Case*

Fig.1 shows the use case of the SNS Agency Robot. After setting this robot at an elderly person's house, for example, an

![](_page_1_Figure_8.jpeg)

Fig. 1. Use case of SNS Agency Robot

elderly person can send a granddaughter a message like "Happy birthday, Hanako! I sent you the present." just by speaking to the SNS Agency Robot. This message will be sent to the granddaughter's LINE account automatically, so that she can see these messages using her accustomed LINE and a smartphone during her spare time. Then, the replied text message using LINE like "Thanks Grandpa!" by the granddaughter will be sent to the elderly person as voice by the SNS Agency Robot. In the same way, when the elderly person speaks to the robot like "Ms. Yamada, when will you come here?", this message will be sent to the care manager's LINE account automatically. The elderly person can also hear the response from the care manager like "I will go there at three pm!". Using the SNS Agency Robot, elderly people can communicate with younger generation interactively via LINE using neither smartphones nor personal computers. Younger generation can also communicate with elderly people interactively using their accustomed LINE and smartphones during their spare time.

#### *B. Message Destination Estimation Method*

 We need to prepare a classification model in advance to realize the message destination estimation according to message contents. We also need to make a classification model against each elderly person. However, it would be difficult to collect needed training data for making a classification model in advance. Therefore, we introduce the message exchange learning-type classification model making method. In this method, we do not have to gather all needed training data in advance. Machine learning performance will be increased gradually by exchanging a message frequently. In this situation, we could not put the responsibility on elderly people. Therefore, we designed the method that uses a response against a message from elderly people as training data.

 Fig.2 shows the message exchange learning-type classification model making method. Firstly, we try to calculate the message destination address probability against the message, "Ms. Yamada, when will you come here?" that is sent by the elderly person. We call this function the Destination Estimation. In the case of Fig.2, the destination address probability is under a predefined threshold value, so that this message will be distributed to all registered persons (ձ). As a result, only a care manager responded such as "I will go there at three pm!" (ղ). In this point, we decide that the message from the elderly person might be for the care manager, then we register the destination address and the message contents into the classification model (ճ). In this method, the correspondence determination between the messages is the most important issue. In this issue, we employed the chronological order method that we evaluate closeness of the response time according to managing the messages in chronological order.

We show the detail of the message destination estimation method consisted of the Destination Estimation and the Classification Model Making in Fig.3. In the Destination Estimation, we give the message from the elderly person to Natural Language Classifier (NLC) of IBM Watson API series. Then, NLC calculates the message destination address probability for each registered person such as a Net Super, a Granddaughter, and a Care Manager. If each destination address probability were lower than a predefined threshold value, the message would be distributed to all registered persons (ձ). If one of the destination address probabilities were higher than a predefined threshold value, the message would be sent to the only that correspondent. NLC is one of the Watson API, which covers 16 kinds. It performs the class classification of the natural language using deep learning. The class of the sentence comes back when we input a sentence. We regarded this class as a destination address and implemented the Destination Estimation. In the Classification Model Making, if we would have a response (ղ) within a predefined term against the message from an elderly person, we recognized such responder as a destination person of the previous message from an elderly person (ձ). Then, we register the responder's address and the message contents from an elderly person with the Classification Model. If the classification model data collecting term would exceed a predefined term, we transmitted the stored data in the Classification Model to NLC as training data.

### IV. SNS AGENCY ROBOT

#### *A. System Architecture*

We designed the SNS Agency Robot based on the serviceoriented architecture. Fig.4 shows the SNS Agency Robot architecture. In external cloud-based services, we employed LINE as SNS, Google Cloud Speech API of Google Cloud Platform as speech recognition, and Natural Language Classifier of IBM Watson as message destination estimation. In a human-type robot, we used PaPeRo, which stands for "Partner-type-Personal-Robot", is a personal robot developed by Japanese firm NEC Corporation [19]. It is noted for its cute appearance and facial recognition system. We implemented the SNS Agency Robot Main System on the cloud service. This

![](_page_2_Figure_5.jpeg)

Fig. 2. Message exchange learning-type classification model making method

![](_page_2_Figure_7.jpeg)

Fig. 4. SNS Agency Robot architecture

Main System controls all external cloud-based services and PaPeRo. Thanks to this architecture, the external cloud-based service adaptation is very easy because it is enough for us to modify only the application interface part.

#### *B. System Configuration*

We show the SNS Agency Robot system configuration in Fig.5. We assigned the SNS Agency Robot Main System to Microsoft Azure, also assigned the SNS Agency Robot Subsystem to Raspberry Pi, which is a single board computer embedded in PaPeRo. These Main System and Subsystem are communicating with each other to execute all functionalities. The Main System provides mainly the LINE message exchange function and message destination estimation function. The Subsystem offers mainly interface function between the Main System and PaPeRo, which has user interface devices like a speaker, camera, proximity sensor, and button.

## *C. Use Case of Prototype System*

We show the use case of the prototype system according to the use case described in Fig.1. When an elderly person speaks "Happy birthday, Hanako! I sent you the present." in front of PaPeRo a still image, a voice message, and a text massage of an elderly person will be appeared on the screen of a granddaughter's smartphone as LINE messages (Fig.6(a)). Then, the replied text message using LINE like "Thanks Grandpa!" by the granddaughter will be sent to the elderly person by the SNS Agency Robot (Fig.6(b)). Then, the ears of PaPeRo will shine, so that the elderly person can know that new messages have arrived. When the elderly person closes to PaPeRo, PaPeRo starts to speak automatically "Thanks Grandpa!". Then, the confirmation message will be sent back to the granddaughter automatically, so that the granddaughter can confirm whether the elderly person has heard the message or not.

#### V. EXPERIMENTS AND DISCUSSION

#### *A. Experiment Outline*

We had an experiment to evaluate our prototype system from 14 Nov. 2016 to 27 Dec. 2016 at the house for the elderly with the care service, named Mon-san Nagasaki in Togitsu-machi, Nagasaki prefecture. The test subjects were a 78 years old woman, 87 years old man, and 88 years old woman. They could not use smartphones. We call the 78 years old woman Ms. A. Before starting experiment, we did some tasks listed in the bellow as experiment preparation.

![](_page_3_Figure_7.jpeg)

- We registered LINE messaging API bot accounts for each test subject's PaPeRo with LINE server.
- We sent communications partners an instruction and a QR code to register a LINE account for PaPeRo with LINE application of their smartphones.
- We installed PaPeRo at the living room of each test subjects and connected PaPeRo with the Internet through Wi-Fi router.
- We explained PaPeRo usage to test subjects by showing demonstration.

 In the case of Ms. A, we asked her daughter lived in different prefecture, a care worker of Mon-san Nagasaki, and our research staff to register the LINE account for PaPeRo. Just after starting experiment, all test subjects enjoyed using PaPeRo. Unfortunately, the physical condition of 87 years old man and 88 years old woman turned worse during experiment period. Therefore, we decided to evaluate the communication history of Ms. A. In this paper, the elderly person's message destination estimation method is main issue. Therefore, we evaluated the speech recognition accuracy that became a premise of the elderly person's message destination estimation method and message destination estimation accuracy. We show the results in the next section.

## *B. Evaluation Results*

At first, we evaluated the speech recognition accuracy. The experiment conditions are shown in the following.

- Target data is the messages from Ms. A.
- Data collection period is from 14 Nov. 2016 to 22 Dec. 2016.
- Target message number is 126.

 We made the correct data manually by hearing all voice messages. In advance of calculating speech recognition accuracy, we divided each message into every word by using morphological analysis. Calculating formula of the speech recognition accuracy is described in formula (1).

$$
Speedh Recognition Accuracy = \frac{\#C - \#I}{\#C + \#S + \#D} \quad \cdots \quad (1)
$$

In the results, #C was 2161, #S was 74, #I was 6, and #D was 147. Total word number was 2388, so that speech recognition accuracy was 90.5%. This accuracy is for Google Speech Recognition API, it is not for our own original function. However, this accuracy affects the precision of the elderly person's message destination estimation method because this method is based on the speech recognition results. Therefore, we evaluated this accuracy in advance of evaluating the message destination estimation accuracy. We judged that 90.5% accuracy is good enough to proceed to the next step, because if we could execute the elderly person's message destination training for long term, we could make the affection of miss speech recognition minimized.

Secondly, we evaluated the elderly person's message destination estimation method. The experiment conditions are shown in the following.

- Target data is the messages from Ms. A.
- Data collection period is from 14 Nov. 2016 to 18 Dec. 2016.
- The predefined term of the response time against Ms.

![](_page_4_Figure_19.jpeg)

Fig. 7. Training data and Classification Model

![](_page_4_Figure_21.jpeg)

| Estimation Results | Experiment<br>term | $21$ Nov. $-$<br><b>27 Nov.</b><br>(Second<br>week) | 28 Nov.-<br>4 Dec.<br>(Third<br>week) | $5$ Dec. $-$<br>11 Dec.<br>(Fourth<br>week) | $12$ Dec. $-$<br>18 Dec.<br>(Fifth<br>week) |
|--------------------|--------------------|-----------------------------------------------------|---------------------------------------|---------------------------------------------|---------------------------------------------|
|                    | Daughter           | $15/15=$<br>100%                                    | $15/15=$<br>100%                      | $4/4=$<br>100%                              | $7/7=$<br>100%                              |
|                    | Research<br>staff  | $0/8 = 0%$                                          | $0/3 = 0%$                            | $0/10=0%$                                   | $2/2=100$<br>$%$                            |
|                    | Care worker        | $0/8 = 0%$                                          | $0/2=0%$                              | $0/2=0%$                                    | $0/2=0%$                                    |
|                    | Total              | $15/26=$<br>57.6%                                   | $15/20=$<br>75.0%                     | $4/16=$<br>25.0%                            | $9/11 =$<br>81.8%                           |
| Correct data       | Daughter           | 15                                                  | 15                                    | 4                                           | 7                                           |
|                    | Research<br>staff  | 8                                                   | 3                                     | 10                                          | 2                                           |
|                    | Care worker        | 3                                                   | $\overline{2}$                        | $\overline{2}$                              | $\overline{2}$                              |
|                    | Total              | 26                                                  | 20                                    | 16                                          | 11                                          |

Fig. 8. Correct data and destination estimation results

A's message (described in Fig.3) is 24 hours. If a communications partner responded to Ms. A's message within 24 hours, the first responder would be registered into the Classification Model.

- The predefined period of the classification model data collecting term (described in Fig.3) is one week. At every week-end, the stored data in the Classification Model is transmitted to NLC as training data (Fig.7). In this mean, at the end of the fourth week, NLC should grow wise.
- We used the exchange messages from the second week to the fifth week as testing data (at the gray part of Fig.7). For example, the destination address of the second week messages will be calculated by NLC using the classification model made by the first week training data.
- We could get the destination probability of each destination candidates from NLC. The probability of total destination candidates becomes 100% without depending on the number of destination candidates. Therefore, we chose 50% as the threshold value described in Fig.3.
- We made the correct data that means the destination address of Ms. A's message manually by checking all message contents and the message exchange context. We show the correct data at the lower column of Fig.8.

According to these conditions, we evaluated the message destination estimation accuracy (Fig.8). We calculated the ratio that we were able to estimate for the correct data definitely (at the gray part of Fig.8). We show the time transient graph of the destination estimation accuracy in the upper part of Fig.8. In this graph, we can see that the fourth week accuracy is temporarily down. We had many messages to our research staff in this week compared with the previous weeks. Therefore, we thought that the learning effect of the past message exchange had not provided yet. It is the evidence that the destination estimation accuracy rises again in the fifth week. From these results, it could be said that our proposed method in this paper is effective for the message destination estimation.

#### VI. CONCLUSION

We proposed the SNS Agency Robot that can be used for the interactive communication between elderly people and younger generation via LINE. In our robot system, elderly people can communicate only by voice due to realizing the simple user interface. In order to determine a LINE message destination address only by voice, we proposed the message exchange learning-type destination estimation method. We also designed the SNS Agency Robot based on the serviceoriented architecture that enables us easily to use external cloud-based services such as LINE messaging API, Google Cloud Speech API, and IBM Watson Natural Language Classifier. We developed the prototype system including the message exchange learning-type destination estimation method on Microsoft Azure. Then, we had the demonstration experiment to evaluate our prototype system at the house for the elderly with the care service in Nagasaki prefecture. In the results of the demonstration experiment, we confirmed that we were able to achieve the message destination estimation probability of more than 80% at the last period of the demonstration experiment. This result proves the effectiveness of our proposed method.

#### ACKNOWLEDGMENT

This work was supported by Strategic Information and Communications R&D Promotion Programme (SCOPE) Grant Number 152310005.

#### REFERENCES

[1] Aoki, E., Yoshitake, S., Kubo, M.: Study on a Nursing System Using Information Communication Technology, Proc. The 8th International Conference on Complex, Intelligent, and Software Intensive Systems (CISIS-2014), pp. 631-636 (2014).

[2] Kato, D., Yamagishi, H., Suzuki, H., Konaka, E., Watanabe, A.: Proposal of a remote watching system utilizing a smartphone and sensors, Proc. 11th International Symposium on Communications and Information Technologies (ISCIT 2011), pp. 36-41 (2011).

[3] Tang Yi Ping, Deng Fei ; Xiong Jian Ying : The investigation of the elder's monitoring system based on life supplying line, Proc. IEEE International Conference on Industrial Technology, pp. 314-318 (2005). [4] Kobayashi, T., Katsuragi, K.: Social Media Mediation System for Elderly People, Proc. IEEE International Conference on Consumer Electronics (ICCE), pp.212-213 (2016).

[5] Kobayashi, T., Katsuragi, K., Arai, K., Sakai, T., Fujimura, M.: Social Media Mediation System for Closing Intergenerational Communication Gap, the 4th IEEE International Workshop on Consumer Devices and Systems (CDS 2016), pp.288-293 (2016).

[6] LINE, https://line.me/en/

[7] Getting started with the Messaging API,

https://developers.line.me/messaging-api/getting-started9

[8] Kobayashi, T., Katsuragi, K., Arai, K., Sakai, T., Fujimura, M.: Social Media Mediation System for Elderly Pepple-Message Exchange Learning Type Switching Method-, Proc. 2016 19th International Conference on Network-Based Information Systems(NBiS 2016), pp.286-291(2016) [9] Zojirushi I-Pot , http://route246.sotobori.com/?p=336

[10] Murase, Y., Nakakura, T., Ota, Yuko., Sugiura, K., :Constructing Distance Communication Environment to Share Activities Using Network, DiCOMO 2011, Multimedia Distributed Cooperative and Mobile Symposium, CDROM (2011).

[11] Inoue, K., Sasaki, C., Nakamura, M.: Communication Robots for Elderly People and Their Families to Support Their Daily Lives –Case Study of Two Families Living with the Communication Robot, Assistive Technology, IOS Press, 2015, pp.980-983 (2015).

[12] Sasama, R., Yamaguchi, T., Yamada, K.: An Experiment for Motivating Elderly People with Robot Guided Interaction, Universal Access in HCI, Part II, HCII 2011, LNCS 6766, pp.214-223 (2011).

[13] Kanoh, M., Oida, Y., Nomura, Y., Araki, A., Konagaya, Y., Ihara, K., Shimizu, T., and Kimura, K.: Examination of Practicability of Communication Robot-Assisted Activity Program for Elderly People, Journal of Robotics and Mechatronics, Vol.23 No.1, pp.3-12 (2011).

[14] Amazon Echo, https://www.amazon.com/Amazon-Echo-Bluetooth-Speaker-with-WiFi-Alexa/dp/B00X4WHP5E

[15] Google Home, https://madeby.google.com/home/

[16] pepper, http://www.softbank.jp/en/robot/

[17] Xin Jin, Anbang Xu, R. Bie, Xian Shen, Min Yin: Spam email filtering with bayesian belief network: using relevant words, IEEE International Conference on Granular Computing, pp. 238-243 (2006)

[18] Sunil B. Rathod, Tareek M. Pattewar: Content based spam detection in email using Bayesian classifier, International Conference on Communications and Signal Processing (ICCSP), pp.1257-1261 (2015)

[19] PaPeRo, https://en.wikipedia.org/wiki/PaPeRo