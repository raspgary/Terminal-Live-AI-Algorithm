# Terminal Live AI Algorithm
This is an algorithm that my team and I built for the Terminal Live AI competition hosted by Correlation One and Citadel. Our algorithm is in the python-algo folder under the name algo_strategy.py. The game is in a tower defense format where there are defensive units and offensive units. The main goal of our algorithm is to first build a defensive infrastructure then start attacking in reactive intervals. If a previous attack did not breach the enemy defenses, then the interval between attacks widens to accumulate more attacking units for larger attacks. There is also a reactive defense algorithm for reacting to enemy attacking units breaching the main defense. Excess resources are used to build a cannon of beacon units to power up attackers. #### Directions from the website on how to play are in the rest of the README below.*

For more details about competitions and the game itself please check out our
[main site](https://terminal.c1games.com/rules).

## Manual Play

We recommend you familiarize yourself with the game and its strategic elements, by playing manually. Check out [the playground](https://terminal.c1games.com/playground).

## Algo Development

To test your algo locally, you should use the new test_algo_[OS] scripts in the scripts folder. Details on its use is documented in the README.md file in the scripts folder. Using this script and the website features are enough for most users to play the game.

For documentation on the all official algos check out [the doc server](https://docs.c1games.com). This site also details useful configuration settings, and advanced details on the input formatting under "Json Format".

For advanced users you can install java and run the game engine locally, however its recommended to use the website for proper analysis as it has visualization features to help you understand.
Java 10 or above is required: [Java Development Kit 10 or above](http://www.oracle.com/technetwork/java/javase/downloads/jdk10-downloads-4416644.html), if you cannot download java 10 just download the most recent java version.

If you are running Windows, you will need Windows PowerShell installed. This comes pre-installed on Windows 10.
Some windows users might need to run the following PowerShell commands in adminstrator mode (right-click the 
PowerShell icon, and click "run as administrator"):
    
    `Set-ExecutionPolicy Unrestricted`
    
If this doesn't work try this:
    
    `Set-ExecutionPolicy Unrestricted CurrentUser`
    
If that still doesn't work, try these below:
    
    `Set-ExecutionPolicy Bypass`
    `Set-ExecutionPolicy RemoteSigned`
    
And don't forget to run the PowerShell as admin.

## Uploading Algos

Zip your algo with the platform-appropriate `zipalgo` binary, found in the `scripts` directory. This
will generate a deflated zip archive, details are provided in the [documentation in the scripts directory](https://github.com/correlation-one/AIGamesStarterKit/tree/master/scripts). 

For example, you can run:

./scripts/zipalgo_mac python-algo my-python-algo.zip

## Troubleshooting

For detailed troubleshooting help related to both website problems and local development check out [the troubleshooting section](https://terminal.c1games.com/rules#Troubleshooting).

#### Python Requirements

Python algos require Python 3 to run. If you are running Unix (Mac OS or Linux), the command `python3` must run on 
Bash or Terminal. If you are running Windows, the command `py -3` must run on PowerShell.
   
#### Java Requirements

Java algos require the Java Development Kit. Java algos also require [Gradle]
(https://gradle.org/install/) for compilation.
   
## Running Algos

To run your algo locally or on our servers, or to enroll your algo in a competition, please see the [documentation 
for the Terminal command line interface in the scripts directory](https://github.com/correlation-one/AIGamesStarterKit/tree/master/scripts)
