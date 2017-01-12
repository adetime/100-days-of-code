# 100 Days Of Code - Log

### Day 1: January 03, 2017


**Today's Progress**: Started #100DaysOfCode Challenge. My first project is cloning an app called DayBreak, which is developed by Hello Sunday Morning's team. It is an app to help people to overcome alcohol problems. Today, I worked on icon mood component, which is based on a stateless React Native component.

**Thoughts:** I really struggled with some tricks on React Native for granting shareability of the code, but the hardest part was make the result UI works on both Android and iOS.

**Link to work:** [Day Break Clone](https://github.com/adetime/day-break-clone)


### Day 2: January 04, 2017


**Today's Progress**: Started to include Mood-Card component. It will have 3 sections, or child components - Header, Short Description, and Footer. The Header component is almost completed, but I still have to think about how to make it more reusable.

**Thoughts:** Make this app has been challenging and exciting. I know that are so many improvements to do, but I think the dots are beginning to connect.   

**Link to work:** [Day Break Clone](https://github.com/adetime/day-break-clone)


### Day 3: January 05, 2017


**Today's Progress**: Started to work on a social-bar component. It will be the Card's footer, enabling users visualize how much likes and comments one post has.

**Thoughts:** Today, I made a huge mistake with setState method. Although I know exactly how setState works, I called this.setState = { something: newValue}. After more than one hour looking for why my component was not re-rendering, I saw this silly mistake. So, always remember: setState is a method, and if your component is not updating after setState is called, odds are that you are not doing this.setState({ something: newValue }).         

**Link to work:** [Day Break Clone](https://github.com/adetime/day-break-clone)


### Day 4: January 06, 2017


**Today's Progress**: Updated the social-bar component, enabling the user gives likes. When a user taps the like button, the button's image change.

**Thoughts:** Although this version of the social-bar is working enough well, I still need to figure out how properly create a reusable button which has both image and title as children.

**Link to work:** [Day Break Clone](https://github.com/adetime/day-break-clone)


### Day 5: January 07, 2017


**Today's Progress**: Worked helping a friend in a new personal project. It will be an app for social dating. Was created the basic layout of Card, Header, and Footer components.

**Thoughts:** Work with flex-like style is really interesting. But, I still need to carefully verify how to make the app layout looks similar on tablet screens. Maybe the problem is on assets - the images are not available in more than one resolution yet.  

**Link to work:** [Vallone-App](https://github.com/adetime/vallone-app)


### Day 6: January 08, 2017


**Today's Progress**: Worked helping a friend in her project to create a new app for social dating. Was created the CardList component, and made some improvements on the Card component.

**Thoughts:** My friend is still think about the app layout. So, for now, we are trying to make our code almost independent of the future layout.  

**Link to work:** [Vallone-App](https://github.com/adetime/vallone-app)



### Day 7: January 09, 2017


**Today's Progress**: Started to work on scale factors to normalize font and image size., etc

**Thoughts:** I need to make more test on recent devices, like iPhone 7, to see with the PixelRatio helper is working well to permit a great look on great range of devices.

**Link to work:** [Day Break Clone](https://github.com/adetime/day-break-clone)

### Day 8: January 10, 2017


**Today's Progress**: Started the SocialBar component and handled its layout in accordance to developed UI design.

**Thoughts:** When we have, at least, a clear direction to follow, everything become easier. Today, the UI design was our facilitator, although it is still a drafting.   

**Link to work:** [Vallone-App](https://github.com/adetime/vallone-app)


### Day 9: January 11, 2017


**Today's Progress**: I found a problem with flexbox on Android. Then, I created another little project to reproduce the unexpected behavior and isolate the problem until find its root cause. I already know how to fix it, but I have to study more deeply to understand why this problem not occur on iOS devices.  


**Thoughts:** The problem occurs when we have a wrapper View container with styles properties given by { flex: 1, alignSelf: 'center'} without no other dimension given. So, if the wrapper View has a child Image component with { width: 350} we will find problems with flexbox on Android devices - particularly on Motorola X play. In that case, If the wrapper view has another view component as child, flexbox properties as justifyContent will break with the following values: 'flex-end', 'space-between', and 'space-around'.    

**Link to work:** [Fexbox-Test](https://github.com/adetime/flexbox-test)
