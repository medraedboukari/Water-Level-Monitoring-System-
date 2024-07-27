<h1>Water Level Monitoring System for  Reservoirs</h1>

<h2>Description</h2>

<p>This project involves developing a real-time water level monitoring system using a Raspberry Pi, an HC-SR04 ultrasonic sensor, and a capacitive water level sensor. The primary objective of this prototype is to measure and monitor the water level in  reservoirs.</p>

<h2>Features</h2>
<ul>
  <li><strong>Ultrasonic Distance Measurement:</strong> Utilizes the HC-SR04 ultrasonic sensor to measure the distance to the water surface.</li>
  <li><strong>Water Level Detection:</strong> Employs a capacitive water level sensor to detect the presence or absence of water.</li>
  <li><strong>Real-Time Monitoring:</strong> Continuously measures and reports the water level, providing real-time data.</li>
  <li><strong>GPIO Configuration:</strong> Configures GPIO pins on the Raspberry Pi for accurate data reading from the sensors.</li>
  <li><strong>Python Implementation:</strong> Uses Python for sensor integration, data processing, and reporting.</li>
</ul>

<h2>Components</h2>
<ul>
  <li>Raspberry Pi</li>
  <li>HC-SR04 Ultrasonic Sensor</li>
  <li>Capacitive Water Level Sensor</li>
  <li>Connecting Cables</li>
</ul>

<h2>How It Works</h2>
<ol>
  <li><strong>Sensor Integration:</strong> The HC-SR04 ultrasonic sensor and the capacitive water level sensor are integrated with the Raspberry Pi.</li>
  <li><strong>Distance Measurement:</strong> A Python program is designed to measure the distance to the water surface using the ultrasonic sensor.</li>
  <li><strong>Water Level Detection:</strong> The capacitive sensor detects the presence or absence of water.</li>
  <li><strong>Data Reporting:</strong> The system continuously monitors and reports the water level distance and status in real-time.</li>
</ol>

<h2>Usage</h2>
<ol>
  <li><strong>Set up the hardware:</strong> Connect the sensors to the Raspberry Pi according to the specified GPIO pins.</li>
  <li><strong>Run the Python script:</strong> Execute the provided Python script to start the real-time monitoring system.</li>
  <li><strong>Monitor the output:</strong> The distance to the water surface and the water level status will be printed to the console.</li>
</ol>

<h2>Code</h2>
<p>The Python script can be found in the repository. It includes functions to measure the distance using the HC-SR04 sensor and to check the status of the water level sensor.</p>

<h2>License</h2>
<p>This project is licensed under the MIT License.</p>


