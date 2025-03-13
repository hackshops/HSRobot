# HSRobot
This repository contains the source code for the HSRobot projects. 

HSRobot is a programming platfom to help learn programming in a unique way. I believe, most conventional programming is taught backwards. Pick up any programming book and they bore you to death taking about variables, loops, control structures, functions and a ton of stuff that's hard to understand, expecially if you are comming from a non-programming background. 

HSRobot takes a different approach. The lessons learned while running a local Girls Who Code Club have been used to build a programming platform that is fun, engaging and easy to learn.

[Raspberry Pi](https://www.raspberrypi.org/) is a powerful and cheap computer that comes with everything you need to learn programming. The ability to interface with hardware and interact with it via programming makes it easier to understand programming concepts.

![HS Robot](https://github.com/hackshops/HSRobot/blob/main/images/HSRobotSideView.png)

![HS Robot](https://github.com/hackshops/HSRobot/blob/main/images/HSRobotTopView.png)

The key components used in HSRobot are:
- [4WD Smart Robbot Car](https://www.digikey.com/en/products/detail/seeed-technology-co-ltd/110090263/10290284)
- [Raspberry Pi](https://www.raspberrypi.org/)
- [L298N Motor Controller](https://www.amazon.com/HiLetgo-Controller-Stepper-H-Bridge-Mega2560/dp/B07BK1QL5T/ref=sr_1_2_sspa?crid=C7DJFXJ145DQ&dib=eyJ2IjoiMSJ9.hK2FjV8Ukp8CCyVTI1seMk4n3aguoO_lNXX3xoiH-O2ps-pSB4GOC_CFp6gAAIK7SKWq0uzWc1NnqY8HWKdgSiW66tFSotzp_4s2rWoBJQJ8-AqIoMtqAfALI6oKtjqiqqNla_iqfg6VdAS6lsJJwsCoRt5YOGw4hNP1K0ajcNFLAbZBV9Nb4NVQFP3stSVCRyYauN3-zrW1AIaqcjZLHwKUO9blNVlM8e-E458fPOM.0Hz8XjjtYPCD7K9C68Dy_BD9UG5BkOTCJkZXelfzydU&dib_tag=se&keywords=L298N&qid=1736107651&sprefix=l298n%2Caps%2C186&sr=8-2-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)
- [Breadboard Jumper Wires](https://www.amazon.com/s?k=breadboard+jumper+wires&crid=87JA053YMU4S&sprefix=breadboard+%2Caps%2C158&ref=nb_sb_ss_ts-doa-p_3_11)

## Useful Links
- [Raspberry Pi Pinout](https://pinout.xyz/)
- [Raspberry Pi GPIO](https://raspberrytips.com/raspberry-pi-gpio-pinout/)

## HSRobot Wiring Diagram

![HSRobot Wiring Diagram](https://github.com/hackshops/HSRobot/blob/main/images/HSRobot-Wiring-Digram.png)

The GPIO Pins used in this project are:
- Pin 18 - Control Left Motors (High to run motors; Low to stop motors)
- Pin 14 and 15 - Control the direction of motors
- Pin 25 - Control Right Motors (High to run motors; Low to stop motors)
- Pin 23 and 24 - Control the direction of motors

## How to Use GPIO Pins to control the motors
| Action | GPIO Pin Value |
|-----------|------------|
| Turn Left Motors Forward | 18 High, 14 Low, 15 High | 
| Turn Left Motors Backward | 18 High, 14 High, 15 Low | 
| Turn Right Motors Forward | 25 High, 23 Low, 24 High | 
| Turn Right Motors Backward | 25 High, 23 High, 24 Low | 
| Stop Motors | 18 Low, 14 Low, 15 Low, 25 Low, 23 Low, 24 Low |

# I got a HackShops Robot Kit! What do I do next? 
Congratulations! HSRobot is a programmn platform and you will have endless fun learning programming.

Follow the [Getting Started Guide](https://github.com/hackshops/HSRobot/blob/main/GettingStarted.md) to get started. 
