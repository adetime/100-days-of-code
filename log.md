# 100 Days Of Code - Log

### Day 1: January 03, 2017


**Today's Progress**: Started #100DaysOfCode Challenge. My first project is cloning an app called DayBreak, which is developed by Hello Sunday Morning's team. It is an app to help people to overcome alcohol problems. Today, I worked on icon mood component, which is based on a stateless React Native component.

**Thoughts:** I really struggled with some tricks on React Native for granting shareability of the code, but the hardest part was make the result UI works on both Android and iOS.

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 2: January 04, 2017


**Today's Progress**: Started to include Mood-Card component. It will have 3 sections, or child components - Header, Short Description, and Footer. The Header component is almost completed, but I still have to think about how to make it more reusable.

**Thoughts:** Make this app has been challenging and exciting. I know that are so many improvements to do, but I think the dots are beginning to connect.   

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 3: January 05, 2017


**Today's Progress**: Started to work on a social-bar component. It will be the Card's footer, enabling users visualize how much likes and comments one post has.

**Thoughts:** Today, I made a huge mistake with setState method. Although I know exactly how setState works, I called this.setState = { something: newValue}. After more than one hour looking for why my component was not re-rendering, I saw this silly mistake. So, always remember: setState is a method, and if your component is not updating after setState is called, odds are that you are not doing this.setState({ something: newValue }).         

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 4: January 06, 2017


**Today's Progress**: Updated the social-bar component, enabling the user gives likes. When a user taps the like button, the button's image change.

**Thoughts:** Although this version of the social-bar is working enough well, I still need to figure out how properly create a reusable button which has both image and title as children.

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 5: January 07, 2017


**Today's Progress**: Worked helping a friend in a new personal project. It will be an app for social dating. Was created the basic layout of Card, Header, and Footer components.

**Thoughts:** Work with flex-like style is really interesting. But, I still need to carefully verify how to make the app layout looks similar on tablet screens. Maybe the problem is on assets - the images are not available in more than one resolution yet.  

**Link to work:** [Vallone-App](https://github.com/adetime/vallone-app)


### Day 6: January 08, 2017


**Today's Progress**: Worked helping a friend in her project to create a new app for social dating. Was created the CardList component, and made some improvements on the Card component.

**Thoughts:** My friend is still think about the app layout. So, for now, we are trying to make our code almost independent of the future layout.  

**Link to work:** [Vallone-App](https://github.com/adetime/valloneapp)



### Day 7: January 09, 2017


**Today's Progress**: Started to work on scale factors to normalize font and image size., etc

**Thoughts:** I need to make more test on recent devices, like iPhone 7, to see with the PixelRatio helper is working well to permit a great look on great range of devices.

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)

### Day 8: January 10, 2017


**Today's Progress**: Started the SocialBar component and handled its layout in accordance to developed UI design.

**Thoughts:** When we have, at least, a clear direction to follow, everything become easier. Today, the UI design was our facilitator, although it is still a drafting.   

**Link to work:** [Vallone-App](https://github.com/adetime/vallone-app)


### Day 9: January 11, 2017


**Today's Progress**: I found a problem with flexbox on Android. Then, I created another little project to reproduce the unexpected behavior and isolate the problem until find its root cause. I already know how to fix it, but I have to study more deeply to understand why this problem not occur on iOS devices.  


**Thoughts:** The problem occurs when we have a wrapper View container with styles properties given by { flex: 1, alignSelf: 'center'} without no other dimension given. So, if the wrapper View has a child Image component with { width: 350} we will find problems with flexbox on Android devices - particularly on Motorola X play. In that case, If the wrapper view has another view component as child, flexbox properties as justifyContent will break with the following values: 'flex-end', 'space-between', and 'space-around'.    

**Link to work:** [Fexbox-Test](https://github.com/adetime/flexbox-test)


### Day 10: January 12, 2017


**Today's Progress**: Solved the problem with flexbox on Android. In fact, it was not an Android specific problem.

**Thoughts:**  It had not seen visible on iOS devices because they have width screens larger than the width of one child image. But, when the width of that image becomes larger we had the same behavior on any device. I found 2 quick ways to solve it: define the image width equals to device width, or remove alignSelf = 'center' property of the wrapper component - alignSelf overrides alignItems behavior in the parent component.    


**Link to work:** [Fexbox-Test](https://github.com/adetime/flexbox-test)



### Day 11: January 13, 2017


**Today's Progress**: Created a better button version. The social bar looks as expected. The Body component of the card was created.

**Thoughts:** It was a really cool day!!! At 5:15am I am going to bed so happy. Hopefully, I will have more code days like this :-)

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 12: January 14, 2017


**Today's Progress**: Created ListCard component using ScrollView and map helper. Also, both Fake-API and FAKE-data were generated to seed multiple cards.

**Thoughts:** The home screen is almost completed! Sooner, I will include interesting things as Redux/Apollo/Firebase. Going to bed 7:00am!

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 13: January 15, 2017


**Today's Progress**: I Made a simplified version of ListCard component, and powered it by ListView. The reason to choice ListView, rather than ScrollView is because ListView can give us a more performant solution. It is totally related with their render strategy. On one hand, ScrollView renders the entire list even with a row is not visible. On the other hand, ListView renders just the part viewed, and does every management necessary to accomplish it behind the scenes.

**Thoughts:** Building natives apps with React Native is really cool. Also, I figured out early that there is not more important and meaningful than test you own app on real (physical) devices. I think it help you even on creativity process. And if you have opportunity to test on multiple devices it is a bonus, because you will be putting on the table so many insights about what the limitations of your app are and how to overcome them.       

**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 14: January 16, 2017


**Today's Progress**: I made some improvements on both Header component and Fake-API. The Header now is more generic and also works well when there is not an icon as a child component. The Fake-API is simpler than before, allowing a more direct way to access specific pieces of data. I also started to build the CardDetail component.

**Thoughts:** I think that I will use a simple ScrollView to list comments on CardDetail. The reason is because the number of comments on one single card is not enough relevant to use a more complex component as a ListView.  
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 15: January 17, 2017


**Today's Progress**: Today I finished the main components of CardDetail's screen, and started to play with Router on the app.

**Thoughts:** I am using react-native-router-flux to manage app's router. That library seems to be very well developed, allowing customization of many of its behaviors and styles. One interested thing that I saw was that the default 'duration' of animation between scene transitions is 150 ms (mile-seconds). Although it is a short amount of time, it is enough time to human's eyes to detect slow motion. So, at the first play of router transition I thought "maybe it is so slow because this animation needs a level of performance that we do not have on simulator". But, even running the app directly on my physical devices, the feeling of lazing was the same. So, I jumped into the source code of the library and the light started to coming from. That 'duration' property can be customized! Then, I give to it the value of one mile-second (duration={1}). After that, transitions between scenes occurs as smooth as we can expect from a native app. I do not know why the authors of react-native-router-flux chosen that big duration. But, I am grateful that they give us the possibility to opt for a different value.        
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 16: January 18, 2017


**Today's Progress**: Today I finished the main components of CommentCreate's screen: Input and InputForm.

**Thoughts:** I already have the majority of components need to reproduce basics user experience on the app. So, will start to clean up the code and organize all together because I think that it is time to moving on to the wonderful Redux' world!
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 17: January 19, 2017


**Today's Progress**: Today I made a deeply review of the code. After a lot of simplification, the code is cleaner.

**Thoughts:** I think that anyone should make times to times a cleaning up of their code. It is interesting as we can see ourself code from a different point of view, just give one or to day.   
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 18: January 21, 2017


**Today's Progress**: Today I started to organize all the app structure to deal with authentication/data persistence (firebase), and to manager the state by Redux.

**Thoughts:** Yesterday I had a problem with babel/async/await. I tried to solve it following tip on stackoverflow, babel docs and opened/closed issues on github. Unfortunately, async/await is something still new, and with little indication of how to solve the problem that I was dealing. So, for now, I decided to put off that level of cut-edge strategy to use promise because it is not the main goal of this project. Then, today I am producing to the challenge again after one day without a positive contribution. Hopefully, that kind of problem will stay far away.
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 19: January 22, 2017


**Today's Progress**: Today I started work with FacebookAuthProvider, and fixed the previous problem with async.

**Thoughts:** The problem  with  async was a forgotten keyword function or a fat arrow function used together.
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 20: January 23, 2017


**Today's Progress**: Created a new screen to login with Facebook or email. Also, redux is managing what first screen the user will see when open the app.

**Thoughts:** The login screen's UI was made inspired by iOS version of the real Daybreak app. But, I am specially satisfied with my personal touches to integrate the login with Facebook button.
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 21: January 24, 2017


**Today's Progress**: Made some improvements on actions creators and reducers. Now, the Continue with Facebook's button is called by redux.

**Thoughts:** Today was hard to find a time to coding on this project because  It was a busy day. But, thankfully I worked enough time to evolve the app.     
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 22: January 25, 2017


**Today's Progress**: Just more configuration on Facebook authentication to be consistent with redux's world. Also, studied how to persist on firebase profile data that the user already has on Facebook.

**Thoughts:** The authentication process is evolving well. More some steps and I will start to work in how to avoid an user to has more than one account. On other words, how to aggregate Facebook and Email signing up process in just one user id.
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 23: January 26, 2017


**Today's Progress**: Worked with promises using async/await, try/catch, and firebase.

**Thoughts:** Firebase already give to us for free displayName, photoURL, and email when an user signing with credential given by Facebook. Need to pay more attention to firebase.auth().onAuthStateChanged() because it is triggered every time that we have a change on user authentication state. As a consequence, all next actions can be lost because of that automatic change on the actions stack.   
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)



### Day 24: January 27, 2017


**Today's Progress**: Create a new screen to receive email and password for signing in/up process. Also, made changes on Input component to use vertical label.

**Thoughts:** I made this screen called LoginWithEmail to help me start to configure authentication process on Firebase with email and password. For now, I will keep it simple to focus on authentication process, but LoginWithEmail component needs some hacks to deal better with keyboard aware events.
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)



### Day 25: January 28, 2017


**Today's Progress**: Started authentication with email and password with firebase.

**Thoughts:** Firebase gives to us a special Real Time Listener called onAuthStateChanged() that is fired off every single time that user change their authentication status. So, it allows us to keep the user logged in the app, even if the user had signed up with email and password, anonymously, or by a third part provider.      
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 26: January 29, 2017


**Today's Progress**: Included createCardButton and MoodChoice component.  

**Thoughts:** The createCardButton is a raised-like button. After had made all its implementation on React Native, I discovered that its shadow is not working properly on Android devices. There are various issues about that problem on React Native community. However, there is a possibility to fix it by updating to React Native 0.40 version. Then, I decided to design the button icon with Inkscape already with a shadow included.       
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 27: January 30, 2017


**Today's Progress**: Finished MoodChoice component, and started CardCreate component.  

**Thoughts:** Redux is not the most simple concept to figure out as a project begins. But, after some iterations the big picture starts to be clear, and clear, and clear again. Then, the initial effort is totally valid to allow the app to scale on a more consistent and clear way.  
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)


### Day 28: January 31, 2017


**Today's Progress**: Worked in a SwitchBar component to allow enable/disable features.  

**Thoughts:** The SwitchBar component receives a targetTag and a targetValue to switch to on/off. It uses a Switch native element given to us by React Native. Switch already has out box everything we need: 1) It looks natively different on each platform. 2) It self-controls the on/off value as the Switch UI is tapped.    
**Link to work:** [Daybreak Clone](https://github.com/adetime/daybreak-clone)
