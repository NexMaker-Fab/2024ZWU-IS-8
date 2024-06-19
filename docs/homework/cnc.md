<h1 style="color: #e19cab;">CNC manufacture</h1>
<h2 style="color: #e19cab;">1. CNC in indusrty: machine type, application, material</h2>

### <font size="3"><h3 style="color: #e19cab;">1. CNC milling machine</h3></font>
CNC milling machines (or milling machines) are very similar to CNC milling machines in that they use multi blade cutting tools that rotate relative to the workpiece to create the desired parts. 
- **Application:**
Although CNC milling machines are usually used to **process hard metals and industrial grade materials**, they are more suitable for **cutting soft and delicate materials**, such as **plastic, wood and foam**, and are very suitable for **creating panels, plastic prototypes and molds for injection molding applications**.
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/7a61c2471f67bff9f2377e00e2918ea0c9acc996/images/CNC/CNC%E9%93%A3%E5%BA%8A.webp" alt="Arduino-input" width="1400">

<center>Haas Mini Mill CNC milling machine</center>

### <font size="3"><h3 style="color: #e19cab;">SOP</h3></font>

- Preparation stage:

Make sure you have gone through the necessary training and understand the equipment operating manual.
Before starting the operation, check that the CNC milling machine has been cleaned and there is no visible damage.
Before starting the machine, verify that the work area is safe and free of any objects that may interfere with operation.

- Device startup phase:

Start the equipment correctly according to the Haas Mini Mill operating manual.
Tools and workpieces can be prepared and loaded while waiting for the machine to warm up.

- Using CNC system stages:

Enter or load your CNC program.
Verify that the tool path and other Settings are correct before starting the milling process.

- In the sales stage:

When you run the program, always look at the milling machine to make sure it is correct.
If you find anything unusual, immediately pause the program and fix it as needed.

- Completion and clean-up stages:

After the workpiece is finished, shut down the machine and clean up the machine and work area.
Put all tools and equipment back in place.

**More details：**https://www.haascnc.com/service/troubleshooting-and-how-to/troubleshooting/operation.html



### <font size="3"><h3 style="color: #e19cab;">2. CNC drilling machine</h3></font>
CNC drilling machines are very similar to traditional drilling machines, as they use rotating cutting tools to machine holes on fixed workpieces. However, due to the reliance on CNC technology, CNC drilling machines are more precise and versatile than traditional drilling machines.
- **Application:**
CNC drilling machines can drill holes while achieving a precision tolerance of ± 0.001 millimeters. They are also compatible with **various materials, including metal, plastic, and wood**. In addition, the latest CNC drilling technology features a turret that can accommodate multiple drill bits and allows you to quickly move between them during the manufacturing process. So it is suitable for**manufacturing wheel hubs, gear blanks, and machined shafts**.
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/7a61c2471f67bff9f2377e00e2918ea0c9acc996/images/CNC/%E9%92%BB%E5%BA%8A.png" alt="Arduino-input" width="1200">

<center>HAAS DM-1 drilling machine</center>

### <font size="3"><h3 style="color: #e19cab;">SOP</h3></font>

- Safety preparation:

Ensure that you are wearing safe work clothes and that there are no loose objects on you that can be sucked into the machine. Make sure you are in a clean, well-lit work area.

- Set coordinate system: 

Select an appropriate coordinate system. This can be the machine's default coordinate system, or it can be your custom coordinate system.

- Load tools and materials: 

Safely load tools and set tool length compensation. Load and secure the workpiece.

- Enter program: 

Enter or load the program correctly. It can be programmed manually or loaded with CAD/ CAM-generated programs.

- Validation and testing: 

Before processing, the program is confirmed by empty running and computer simulation. Adjust cutting speed and feed speed.

- Run the program: 

After confirming that everything is ready, start running the program and monitor the process.

**More details：**https://www.haascnc.com/zh/owners/pre-install-guide/mills-pre-install/DM-1.html

Reference web： https://baijiahao.baidu.com/s?id=1774803998423791071&wfr=spider&for=pc

<h2 style="color: #e19cab;">2. How to keep safty</h2>

<h3 style="color: #e19cab;">Detail</h3>

【关于cnc防护-哔哩哔哩】 https://b23.tv/2XURIcR

1. must have a comprehensive understanding of the machine, mechanical properties and transmission system principle, power supply device, certificate to work.
2. every day before work operation, start the machine tool to run at low speed for 5 minutes empty operation, start the production point check, fill in the "equipment point check table" content, check whether the machine tool parts are normal.
3. check the wear, tie the cuffs, wear glasses, do not wear gloves operation, girls need to put the hair on the job with a good cap to avoid accidents.
4. before starting, remove the obstacles and measuring tools on the guide rail and sliding surface, and remove the clamping tool in time. Check whether the mechanical, hydraulic, pneumatic and other operating handles, valves, switches, etc. are in the non-working position, and check whether the tool holder is in the non-working position. Check whether the oil in the box is within the specified scale range, and refuel according to the lubrication chart or instructions.
5. turn on and off in order, start the machine tool and then turn on the CNC system, turn off the CNC system and then turn off the machine tool.
6. the correct tool, determine the workpiece coordinate system, and check the data.
7. the program should be carefully checked after input, including the code, instructions, addresses, values, signs, decimal points and grammar check, to ensure correct.
8, after debugging the program, before the formal cutting, check the program, tools, fixtures, workpieces, parameters, etc., are positive
True.
9. the tool compensation value input, to the knife complement, compensation value, positive and negative signs, decimal point carefully check.
10, according to the process and procedure requirements clamping tool. Before the execution of formal processing, the input program and parameters should be carefully checked, and the program trial run should be carried out to prevent the collision between the tool and the workpiece during processing and damage to the machine tool and the tool.
11, according to the procedure, according to the process of processing, it is strictly prohibited to increase the amount of feed, cutting speed and cutting depth, it is strictly prohibited to use the machine tool with overload and super performance range, it is strictly prohibited to operate in violation of regulations, and it is not allowed to use the precision machine tool for rough machining. The tool should be kept sharp, the knife is not allowed to stop, and the hydraulic system is not allowed to adjust without permission (except the throttle valve).
12. After sharpening the tool and replacing the tool, the tool length should be re-measured and the tool complement value and the tool complement number should be modified.
13, after the modification of the program, the modified part should be carefully calculated and carefully checked.
14, manual continuous feed operation, you must check whether the position selected by the various switches is correct, determine the positive and negative direction, and then operate.
15. Let the machine run empty for more than 15 minutes after starting, so that the machine can achieve thermal balance.
16, once abnormal conditions are found in the operation of the machine tool, the red emergency stop button should be immediately pressed to terminate all movements and operations of the machine tool. After the fault is removed, the machine can be operated again and the program can be executed.
17. When the machine tool alarm occurs, the cause should be identified according to the alarm number and eliminated in time.
18. Regularly clean up the iron filings and other debris in the coolant box, and timely supplement the coolant according to the regulations.
19, without the permission of the workshop supervisor, do not insert U (hard) disk, CD into the CNC machine tool, do not modify or delete the process in the machine tool
Order.
20. after work, clean up the site, clean the iron filings of CNC machine tools, wipe the lathe, oil anti-rust, according to the regulations in the refueling part of the oil, the workpiece on the shelf neatly placed, do 5S work.

Reference web:
1. https://www.tmt.com.tw/cht/news/precautions-for-safety-operation-of-cnc-lathe.html#:~:text=1.%20%E5%AE%89%E5%85%A8%E6%93%8D%E4%BD%9C%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A0%85,%E4%B8%8D%E5%8F%AF%E8%B6%85%E8%B2%A0%E8%8D%B7%E5%8A%A0%E5%B7%A5%E3%80%82
2. https://www.safehoo.com/Item/332371.aspx