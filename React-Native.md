# React Native

## [getting started with react native](https://reactnative.dev/docs/getting-started)




### Name three Core Components of React Native and describe what they do.

1. View: The View component is a fundamental building block in React Native, serving as a container for other components.

1. Text: The Text component is used for displaying text in a React Native application. 

1. Image: The Image component is used for displaying images in a React Native application.

### What problem does React Native solve (why call it native)?

    
React Native is a framework designed to solve the problem of **cross-platform** mobile app development. The term "native" in React Native refers to the fact that it allows developers to build mobile applications that look and feel like they were developed using platform-specific native technologies (e.g., Swift and Objective-C for iOS, Java for Android).

### What are the building blocks of a React Native app? How does that compare to a React app?


The building blocks of a React Native app and a React web app share many similarities, given that React Native is built on top of React. However, there are some key differences due to the nature of mobile and web platforms. 

**Building Blocks of a React Native App:**

1. Components: Components are the fundamental building blocks in both React and React Native. React Native has a set of core components like View, Text, and Image that are specific to mobile app development.

1. Navigator: In React Native, you often use navigation libraries like React Navigation to handle app navigation. 

1. Styling: React Native uses a similar styling approach to React, but with some differences. 

**Building Blocks of a React Web App:**

1. Components: React web apps use React components to define the UI and structure of the application. 

1. Routing: For web applications, you typically use libraries like React Router for handling client-side routing. 

1. Styling: In React web apps, you use CSS for styling, either through traditional CSS files or CSS-in-JS solutions like styled-components.


## [expo](https://expo.dev/)




### What solution does expo provide?

 Expo aims to simplify and accelerate the development process by offering the following solutions:

 1. Development Environment
 1. Managed Workflow
 1. Pre-Built Components
 1. Over-the-Air (OTA) Updates
 1. Expo Go

### Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the **"Managed" workflow**. 

### What is the difference between React Native and Expo?

**React Native:**

* Framework for building mobile apps.
* Offers more control and customization.
* Requires platform-specific setup (Xcode/Android Studio).
* Supports native modules for deep integrations.
* App deployment is done independently.
* Suitable for complex or custom projects.

**Expo:**

* Development environment with streamlined workflow.
* Simplifies development, ideal for beginners.
* Minimizes platform-specific setup.
* Limited to built-in modules (although extensible).
* Offers over-the-air updates for app delivery.
* Great for rapid prototyping and simpler apps.

## [expo snack](https://snack.expo.dev/)

### Checkout this tool. What does snack allow you to do?

Snack allows you to write, run, and preview React Native code in a web browser. It provides access to Expo's APIs, facilitates sharing and collaboration, and is great for prototyping and learning.

## [ejecting](https://docs.expo.dev/archive/glossary/#eject?redirected)




### What does “eject” mean within the context of Expo?


In the context of Expo, "eject" means transitioning from Expo's simplified development environment to a more traditional React Native setup. It's done to gain more control over native code, build configurations, and custom dependencies.

### When should you not eject?


You should avoid ejecting from Expo's Managed Workflow when you want to keep development simple, don't need extensive native code customization, and your app's dependencies are compatible. It's beneficial for rapid prototyping and over-the-air updates.

### Why might you choose to eject?


You might choose to eject from Expo when you need custom native code, advanced build configurations, non-Expo dependencies, platform-specific features, or full control over your project's development and updates

### Tutorial
## [react native basics](https://reactnative.dev/docs/tutorial)