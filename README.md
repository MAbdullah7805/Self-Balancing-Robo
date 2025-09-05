# Self-Balancing-Robo
Being an enthusiast of Robots, I am excited to share my progress in making my fully customized Self-Balancing Robo. The purpose of making this little robo was to learn the real use of microcontrollers in real-life projects. Another reason for building this little guy was to build it using locally available components that are cheaper in cost but operate well. As these cheaper modules are not precise and have many flaws in them, this was a very challenging part for me, and also, the job of an Engineer is to make things possible using very less opportunities.
How this little guy works:
It works on the principle of an Inverted Pendulum. In my words, the principle says “the higher the height, the easier it is to balance.” What if we want to stabilize a pencil or a long stick on our finger? You can find the answer by yourself.
It uses mpu6050’s raw data, filters it, and calculates real angles. The error is calculated using the actual angle and the desired angle. A PID controller is used to stabilize it. The PID controller generates its output, and then this output is used as the PWM signal for the motors. And this keeps running in a loop using a feedback loop. A feedback loop is a system where the output of a process is fed back into the input, influencing future outputs.
And then the story begins to tune the PID constants. This process is very crucial and takes too much time. It took me about 2-3 weeks to stabilize it.
Required components:
i)	A microcontroller, I used ESP32.
ii)	MPU6050 6-axis Gyro + Accelero.
iii)	DC gear Motors.
iv)	L298N Motor driver.
v)	18650 batteries + BMS.
vi)	Frame (build your one or find mine on GitHub).
vii)	Spacers for stack building.
