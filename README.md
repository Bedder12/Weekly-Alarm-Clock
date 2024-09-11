# Weekly-Alarm-Clock
My goal is to develop a graphical application (GUI) for a weekly alarm clock. In this project, I’ll apply basic principles to build a robust and well-structured piece of software. During this exercise, I’ll focus on creating a user-friendly interface with different components while managing the logic behind the weekly alarm clock based on my requirements.

These requirements include allowing the user to set the day, hour, minute, and second separately using buttons or similar controls. The clock will run continuously, and the user will be able to switch between digital and analog time displays. Additionally, it will be possible to view all the alarms that have been set and remove them all with a single button press. The GUI will also show when an alarm goes off.

By combining the interface with the necessary functionality, I aim to create an intuitive and efficient weekly alarm clock.


# Implementation

For the implementation, the program is divided into five packages containing classes and interfaces to make the code more maintainable, reusable, and easy to understand.

2.1 Alarm
In the "alarm" package, there's an Alarm class that represents individual alarms. There's also an interface named AlarmType, which defines the basic functions alarms can perform. Another class, AlarmManager, handles multiple alarms at the same time. This setup makes it easy to manage alarms separately and collectively.

2.2 Clock
The "clock" package contains the main clock class, WeekAlarmClock. This clock uses components like CircularCounter24 and Counter7 to track the time and determine when the alarms should be triggered. Think of it as the clock using different tools to count hours, minutes, and days of the week.

2.3 Counter
The "counter" package provides various counters for handling different time units, such as hours, minutes, and seconds. These counters are essential for ensuring that the time is tracked accurately and that the alarms go off at the right time.

2.4 Time
In the "time" package, there's a Time class used to manage time itself. This package also contains an interface called TimeType, which includes the functions needed to handle different aspects of time.

2.5 Package Summary
This modular structure makes the code easier to extend and modify when needed. Each part has a clear responsibility—for example, Alarm and AlarmManager handle the alarms, while WeekAlarmClock manages the clock itself. The code also uses inheritance to create different counters and interfaces, making it easier to reuse code in different contexts.

It’s like having a customizable digital clock with an adjustable alarm function that can be modified as necessary. This approach ensures that the program is not only functional but also adaptable for future updates or changes.

# Result

We set the current time using a text input, as shown in Figure 1. From the input, we split the text at each ":", separating it into day, hour, minute, and second. The first element (array[0]) is assigned to the day variable, and we create other variables for the hours, minutes, and seconds. Then, we use these variables to create a new instance of the setTime method from our WeekAlarmClock class, passing the variables as shown in Figure 2. Finally, in Figure 3, we can see that the time changes to the new value we set.

Figure 1: (Shows that you can set day, hour, minute, and second)



