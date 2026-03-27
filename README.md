# Spline-2D-Practice-Chicago
Found a few examples of projects other people did within the spline community and recreated aspects of them. This is after my trip to Chicago so I wanted to utilize the pictures I took during the trip.


## The Inspiration
<img width="776" height="441" alt="Screenshot 2026-03-24 at 2 34 35 PM" src="https://github.com/user-attachments/assets/0b7ffc63-c679-4076-bab4-85a60a89a0e3" />
<img width="1096" height="615" alt="Screenshot 2026-03-24 at 2 33 37 PM" src="https://github.com/user-attachments/assets/2e8d7229-30af-45ed-98ba-ddb86c190cfa" />

As someone that loves to 3D model and create physical things, I havent worked much in the mix of 2d graphics with 3D elements. This is something I wanted to explore more, especially with Splines 2D creation tool. I want to implement a lot of 3D elements into my design work in the future and working with these 3D elements that interact with 2D graphics felt like a great way to start.

I chose these two examples to reverse engineer and create my own work using these elements. The first one I worked with was the implementation of a 2D mask that moves, revealing the 2D image inside while also staying on top of text that is moving in the background. The second example is something ive been wanting to learn how to implement into more designs. The liquid glass effect on a 3D object is a really cool collaboration between 3D and 2D that doesn't seem that dificult, especially with the presets provided in Spline.

## Object Masking and Endless Text

### Object Masking
I started this my dissecting each element in the references file. How did they make a mask? Is there anything special I need to do to keep the mask while its spinning? I started with creating a 3D star that I know I want to use as my mask. Once I masked this object with my chosen chicago images, the 3D aspect depth of it seemed to not be visible anymore. Even though the depth was gone, I was still able to affect the x, y, and z axis to make the star move in a way that feels 3D as it diplays as more of a 2D shape. 

Adding movent proved to be very simple, but in order to make the star looking like its endlessly spinning in one direction while changing positions and shape, I need to create 3 states for it to change to. The first and last state were the exact same but this allowed the star to go back to that first state while keeping the same direction of rotation.

As you can see in the video I attached, the star goes through this movement while the images its masking change. I wanted to add this extra element of the design to show the different states of the Chicago city. The images switch fully after 5 seconds and then switch back at 10 seconds, making two passes with the star a complete cycle.

### Endless Text

For the Chicago text that endlessly scrolls in the background of the frame, it was a much easier process than I thought it was going to be. To make the endless scroll happen, you create the text who want to scroll 3 times, "Chicago Chicago Chicago". Create your Base State and a State events in a way where the first Chicago in the Base State and the last Chicago in the State are perfectly aligned with each other. If you make the Event an endless linear transition from Base State to State, this makes the text look endless as it ends and starts at the same spot.

<img width="1144" height="214" alt="Screenshot 2026-03-24 at 2 27 48 PM" src="https://github.com/user-attachments/assets/6e0b0575-94bb-42bf-abab-7049f3152571" />
<img width="2008" height="428" alt="image" src="https://github.com/user-attachments/assets/cf8f8984-287d-4dba-81ee-0a4ca8a07e23" />


## 3D Music is Liquid Glass

The last thing I wanted to add to this project was the liquid glass object. I like the idea of a 3D object that affects the visuals of a 2D graphic and I think liquid glass does this well. I started with selecting a 3D object that I wanted to turn into liquid glass. I decided to do a music note because while I was in Chicago there was an endless amount of sounds but a lot of great live music. This felt very important to my experience in Chicago and I wanted to implement it into my piece.

Make the music note into a liquid glass effect was really easy on Spline. Spline has a lot of presets for materials, including a few glass presets. I chose glass 5 to use because it felt like the most see through and bright, fitting with the overall scene. There was a lot of little tweaks I did with the material settings to get it to look how I wanted. Spline provides a lot of different settings to change the lighting, texture, and other physical aspects of objects, making it easier to make the object look the way you want it.

<img width="1654" height="1520" alt="image" src="https://github.com/user-attachments/assets/62e68bf3-c005-4e5e-a3c1-cd09a4662bf3" /><img width="1144" height="1480" alt="image" src="https://github.com/user-attachments/assets/461bbe4b-eac6-4000-bbdb-644b7a4e7529" />

Once I got the physical look of the glass music note, I worked on giving it motion. I really wanted it to feel like it is bouncing on the edges of the frame, but in a way where its rotation is based on how the music note hits the edge of the frame. In order to do this, I made 

