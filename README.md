# Spline-2D-Practice-Chicago
Found a few examples of projects other people did within the spline community and recreated aspects of them. This is after my trip to Chicago so I wanted to utilize the pictures I took during the trip.


## The Inspiration
<img width="776" height="441" alt="Screenshot 2026-03-24 at 2 34 35 PM" src="https://github.com/user-attachments/assets/0b7ffc63-c679-4076-bab4-85a60a89a0e3" />
<img width="1096" height="615" alt="Screenshot 2026-03-24 at 2 33 37 PM" src="https://github.com/user-attachments/assets/2e8d7229-30af-45ed-98ba-ddb86c190cfa" />

As someone that loves to 3D model and create physical things, I havent worked much in the mix of 2d graphics with 3D elements. This is something I wanted to explore more, especially with Splines 2D creation tool. I want to implement a lot of 3D elements into my design work in the future and working with these 3D elements that interact with 2D graphics felt like a great way to start.

I chose these two examples to reverse engineer and create my own work using these elements. The first one I worked with was the implementation of a 2D mask that moves, revealing the 2D image inside while also staying on top of text that is moving in the background. The second example is something ive been wanting to learn how to implement into more designs. The liquid glass effect on a 3D object is a really cool collaboration between 3D and 2D that doesn't seem that dificult, especially with the presets provided in Spline.

## Object Masking and Endless Text

I started this my dissecting each element in the references file.




### Endless Text

For the Chicago text that endlessly scrolls in the background of the frame, it was a much easier process than I thought it was going to be. To make the endless scroll happen, you create the text who want to scroll 3 times, "Chicago Chicago Chicago". Create your Base State and a State events in a way where the first Chicago in the Base State and the last Chicago in the State are perfectly aligned with each other. If you make the Event an endless linear transition from Base State to State, this makes the text look endless as it ends and starts at the same spot.

<img width="1144" height="214" alt="Screenshot 2026-03-24 at 2 27 48 PM" src="https://github.com/user-attachments/assets/6e0b0575-94bb-42bf-abab-7049f3152571" />
<img width="1144" height="214" alt="Screenshot 2026-03-24 at 2 28 12 PM" src="https://github.com/user-attachments/assets/67448865-70ad-47fd-9d23-b56cb7599605" />
