# Guardian Drive 🚗📱

Guardian Drive is an Android application designed to detect accidents through mathematical calculations of the built-in sensor data on the user's device. It raises alerts to the user within a 30-second window, and if the user fails to respond, the application automatically sends messages to the emergency contacts along with the accident location.

## Features

- Accident Detection: Utilizes advanced mathematical calculations using device sensors to detect potential accidents.
- Alert System: Notifies the user with an alarm and vibration for immediate attention.
- Emergency Contact Messaging: Automatically sends messages to emergency contacts with the accident location if the user doesn't respond within 30 seconds.
- User-Friendly Interface: Provides a simple and intuitive user interface for seamless interaction.

## Algorithm

The Guardian Drive application employs the following algorithm for accident detection:
The given algorithm can be represented in mathematical equations as follows:

Let:
- `combined_weighted_value` be the combined weighted value calculated as `weighted_gForce + weighted_sound + weighted_pressure`
- `threshold_speed` be the threshold value for speed
- `SVP` be the value of SVP
- `ET` be the value of ET
- `MP` be the value of MP

Then the algorithm can be expressed mathematically as:

**Input:** gForce, pressure, speed, sound, SVP, ET, MP  
**Output:** Accident detection result  

1. Calculate the combined weighted value:  
   - **`combined_weighted_value = weighted_gForce + weighted_sound + weighted_pressure`**

2. Check if an accident is detected:  
   - **If** `combined_weighted_value ≥ 1` **and** `speed ≥ threshold_speed`, **then** **return** `true`  
   - **Else if** `combined_weighted_value + (SVP / 2.06) ≥ 3`, **then** **return** `true`  
   - **Else if** `combined_weighted_value ≥ 1` **and** `ET < MP`, **then** **return** `true`  
   - **Else**, **return** `false`  

## Technology Stack

The Guardian Drive application utilizes the following technologies and tools:

-  Java: The primary programming language used for Android application development.
-  Android SDK: Provides the necessary tools and libraries for developing Android applications.
-  Firebase: A comprehensive mobile development platform used for real-time data storage, messaging, and user authentication.
-  Volley: A networking library for handling HTTP requests and responses in Android applications.
-  Glide: An image loading and caching library for Android applications.

## Screenshots



Feel free to explore and use Guardian Drive to enhance safety and raise awareness about road accidents. Your feedback and contributions are highly appreciated! 😄🚗📱

