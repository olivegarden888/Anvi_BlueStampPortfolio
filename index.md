# Three Jointed Robotic Arm
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Anvi G | Windmere Ranch Middle School | Computer Science | Incoming 7th Grader

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> 


For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE 
- 



# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/oB7ArvjD6FY?si=KT3m7q0Yzt7fWj95" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description 

 For my second milestone, I focused on building the robotic arm and connecting the joystick. The arm has three joints, so I used three servo motors one for each joint and also another servo so it can rotate. I also connected the joystick to the Arduino. Later, in Milestone 3, I’ll write the code that makes the arm move using the joystick.

## Challenges

  During this Milestone I had a couple of challenges like first I could not fit a piece into another one so I had to sandpaper it down so it would fit. Anothr challenge that I had was that I didn't screw a screw in properly so because of that the arm was not stable and would not stand on it's own.

## Next Steps

  For my next Milestone I am going to finish coding my robotic arm so it can move whenever I move the joystick.
  
## Schematics

![Headstone Image](circuit_image-3.png)



# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/kOTR2lKDriY?si=Tf3gUGSXZySFV1TE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description

For my first milestone, I tested all the parts like the servos, joysticks, and the Nano Shield to make sure they were working. I connected everything to my computer and ran some simple code to check if the parts worked properly. The servos move using something called a PWM signal. PWM stands for "Pulse Width Modulation," which means the signal quickly turns on and off to control how much power is sent. I connected the servo signal to pin number 7 on the Arduino Shield.

## Challenge
A challenge that I had was that I had to connect two wires together and then when I was heat shrinking the plastic I accidentally burned the wires.

## Next Steps
My plan to finish the project is that first I will build the arm and then after building the arm I will code it.

## Schematics

![Headstone Image](circuit_image-2.png)

## Code

```c++

void loop() {
  // put your main code here, to run repeatedly: #include<Servo.h>
Servo myservo;  // create servo object to control a servo
                 // a maximum of eight servo objects can be created  
int pos = 0;     // variable to store the servo position
void setup()
{
myservo.attach(10);  // attaches the servo on pin 10 to the servo object
}
void loop()
{
for(pos=0;pos<180;pos+=1)  // goes from 0 degrees to 180 degrees 
{
 myservo.write(pos); // tell servo to go to position in variable 'pos'
 delay(15);  // waits 15ms for the servo to reach the position
}
for(pos = 180;pos>=1;pos-=1)  // goes from 180 degrees to 0 degrees
 {
 myservo.write(pos); // tell servo to go to position in variable 'pos' 
 delay(15);  //waits 15ms for the servo to reach the position
 }
}

# Starter Project
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/EDjiuEoxJuI?si=wos0XdUu4kA3OXpi" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

  This is an RGB Slider and it works by first plugging it into a power source. Then using the sliders the colors change. For example when you slide the red slider the the intensity of the color red increases and becomes red, same for the other two sliders. What I did was solder the sliders onto the main chip and also added the power source to the card. Over all this project was simple and helped me learn how to solder and how LEDs work.


# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```


# Bill of Materials

Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
