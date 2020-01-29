# Ros-Startup-Services

Configuration of supervisord to start up the ROS packages on my rover

You will need to install supervisord. I installed from source. https://github.com/Supervisor/supervisor.
Copy the supervisord.conf file to /etc/supervisord and the supervisord.service file to /etc/systemd/system.
Restart systemd
If everything is good you should be able to issue a supervisorctl status command and see the services available.
Roscore should be started and you don't have touchscreen yet so it won't start. All other services should be Stopped.
Edit the files in startup to conform to your robot.
Edit the supervisord.conf file to add in different script names etc.

I'll be creating a repo for the touchscreen part of this project soon. Its for a 4-D systems 43-DT touchscreen. Has gauges for battery voltage, cpu amps, cpu and gpu temp and a configuration screen to set up the launch profile. Also has a resources screen with graphical representation of the cpu cores and gpu cores on the Xavier in the rover.


