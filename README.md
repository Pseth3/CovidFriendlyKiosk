<B> This is a College project for completion of a Master's Degree</B> 

# CovidFriendlyKiosk
Computer vision empowers machines to detect and recognise different objects in the surroundings just like humans. The information derived can be used to make decisions in critical applications. These applications can help safeguard against the spread of harmful diseases by minimising contact with surfaces accessible to the public like touchscreen kiosks in the cafeterias.. This can be achieved by implementing gesture control in the kiosks.

# Introduction
In the pre covid world organisations invested in touch screen kiosks for various applications. But post covid, it does not seem to be a good idea to share the same touchscreen as thousands of others. The objective of this project is to recognise gestures and hand actions using computer vision and based on these actions navigate and operate a food ordering kiosk.

# Problem Statement
In the campus of Virginia Tech alone there are a total of 15 cafeterias that have implemented the technology of touch screen kiosks for ordering. Each cafeteria has about 10 kiosks placed in various locations. Across the United States there are about 4000 colleges and universities, this brings the kiosk count to about 600,000. Increased implementations of touchscreen kiosks in college cafeterias has become a concern for spread of  disease causing germs and bacteria. Since a lot has been spent in the installation of the infrastructure, it is in the best interest to upgrade these with a single camera sensor. This will eliminate the need to touch the kiosks and hence spread of diseases can be stopped along with minimising the financial implications of making the kiosks obsolete.

# Approach
The idea is to develop a software that can be used in the kiosks along with the addition of a camera. For the software design, we found inspiration from the ‘labelimg’ project on Github - https://github.com/tzutalin/labelImg and the youtube channel by Nicholas Renotte.

We will reuse the repository ‘labelimg’ which relies heavily on OpenCV and use the TensorFlow object detection API.

Initially, we will create a catalog of hand gestures that will be used to navigate through the kiosk. Using a camera multiple images will be collected for each gesture to create a diverse dataset. The data set will be labeled using the labelimg library. After creating the data set we will use the tensorflow image detection API to create a model to recognize the different gestures. The final development phase consists of writing a code to implement the workflow of the ordering kiosks using python.