<h1 style="color: #e19cab;">CNC manufacture</h1>

<h2 style="color: #e19cab;">CNC in indusrty</h2>

### <font size="3"><h3 style="color: #e19cab;">1. CNC milling machine</h3></font>
CNC milling machines (or milling machines) are very similar to CNC milling machines in that they use multi blade cutting tools that rotate relative to the workpiece to create the desired parts. 
- **Application:**
Although CNC milling machines are usually used to **process hard metals and industrial grade materials**, they are more suitable for **cutting soft and delicate materials**, such as **plastic, wood and foam**, and are very suitable for **creating panels, plastic prototypes and molds for injection molding applications**.
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/7a61c2471f67bff9f2377e00e2918ea0c9acc996/images/CNC/CNC%E9%93%A3%E5%BA%8A.webp" alt="Arduino-input" width="1400">

<center>Haas Mini Mill CNC milling machine</center>

### <font size="3"><h3 style="color: #e19cab;">2. SOP</h3></font>

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

- In the manufacture stage:

When you run the program, always look at the milling machine to make sure it is correct.
If you find anything unusual, immediately pause the program and fix it as needed.

- Completion and clean-up stages:

After the workpiece is finished, shut down the machine and clean up the machine and work area.
Put all tools and equipment back in place.

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/8698ccd2a64e186ec690e91a7150f65062db8233/images/CNC/CNC%20sop.png" alt="Arduino-input" width="1400">

### <font size="3"><h3 style="color: #e19cab;">3. Process</h3></font>

<h4 style="color: #e19cab;">Metal</h4>

1. Design and programming: 

CAD (Computer aided design) software is used to design parts, and CAM (computer aided manufacturing) software is used to program the machining path. Factors to consider when programming include metal material, cutting force, tool type, tool path, etc.

2. Tool selection: 

According to the processing material and processing content, select the appropriate tool and assembly. Haas's 30+1 side-mounted tool library allows for easy tool change and increased machining efficiency.（Haas's 30+1 side-mounted tool library is an efficient tool changing system that is widely used in CNC machining centers. This tool library can be assembled with various types of tools, including milling cutters, drills, line cutters, boring knives, etc.）

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/deb7372e6e9798b04dc217522c9390a50e8e87be/images/CNC/CNC%E5%88%80%E5%A4%B4.png" alt="Arduino-input" width="1400">

3. Workpiece fixation: 

The metal material to be machined is fixed on the CNC machine, while ensuring the workpiece is safe, stable and accurately aligned.

4. Operation program: 

Run the CAM program written before, observe the operation of the machine tool is normal, to ensure that the processing is safe and effective.

5. Machining: 

CNC machine tools are programmed to process metal workpieces. Possible machining steps include milling, turning, drilling, cutting, etc.

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/a976979b4adce87251b1eb96726b88050104cab3/images/CNC/CNC%E6%9D%90%E6%96%99.png" alt="Arduino-input" width="1400">

6. Acceptance and post-processing:

 After processing, it is necessary to check the quality of the machined parts, including size, tolerance and surface roughness. Post-processing steps such as deburring, polishing, coloring, etc., may be required.

Reference web：
1. https://www.haascnc.com/machines/vertical-mills/mini-mills.html#features
2. https://doc.docsou.com/b4065c70848bbb927ee392cdf.html
3. https://www.youtube.com/watch?v=Sq_9g0-rvTQ


<h2 style="color: #e19cab;">How to keep safty</h2>

<h3 style="color: #e19cab;">1. Detail</h3>

【关于cnc防护-哔哩哔哩】 https://b23.tv/2XURIcR

1. Must have a comprehensive understanding of the machine, mechanical properties and transmission system principle, power supply device, certificate to work.
2. Every day before work operation, start the machine tool to run at low speed for 5 minutes empty operation, start the production point check, fill in the "equipment point check table" content, check whether the machine tool parts are normal.
3. Check the wear, tie the cuffs, wear glasses, do not wear gloves operation, girls need to put the hair on the job with a good cap to avoid accidents.

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/1d76c1f32e0c711be93c3ecbf170c00acd2e6582/images/CNC/CNC1.webp" alt="Arduino-input" width="1400">

4. Before starting, remove the obstacles and measuring tools on the guide rail and sliding surface, and remove the clamping tool in time. Check whether the mechanical, hydraulic, pneumatic and other operating handles, valves, switches, etc. are in the non-working position, and check whether the tool holder is in the non-working position. Check whether the oil in the box is within the specified scale range, and refuel according to the lubrication chart or instructions.
5. Turn on and off in order, start the machine tool and then turn on the CNC system, turn off the CNC system and then turn off the machine tool.
6. The correct tool, determine the workpiece coordinate system, and check the data.
7. The program should be carefully checked after input, including the code, instructions, addresses, values, signs, decimal points and grammar check, to ensure correct.
8. After debugging the program, before the formal cutting, check the program, tools, fixtures, workpieces, parameters, etc., are positive
True.
9. The tool compensation value input, to the knife complement, compensation value, positive and negative signs, decimal point carefully check.
10. According to the process and procedure requirements clamping tool. Before the execution of formal processing, the input program and parameters should be carefully checked, and the program trial run should be carried out to prevent the collision between the tool and the workpiece during processing and damage to the machine tool and the tool.
11. According to the procedure, according to the process of processing, it is strictly prohibited to increase the amount of feed, cutting speed and cutting depth, it is strictly prohibited to use the machine tool with overload and super performance range, it is strictly prohibited to operate in violation of regulations, and it is not allowed to use the precision machine tool for rough machining. The tool should be kept sharp, the knife is not allowed to stop, and the hydraulic system is not allowed to adjust without permission (except the throttle valve).
12. After sharpening the tool and replacing the tool, the tool length should be re-measured and the tool complement value and the tool complement number should be modified.
13. After the modification of the program, the modified part should be carefully calculated and carefully checked.
14. Manual continuous feed operation, you must check whether the position selected by the various switches is correct, determine the positive and negative direction, and then operate.
15. Let the machine run empty for more than 15 minutes after starting, so that the machine can achieve thermal balance.
16. Once abnormal conditions are found in the operation of the machine tool, the red emergency stop button should be immediately pressed to terminate all movements and operations of the machine tool. After the fault is removed, the machine can be operated again and the program can be executed.

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/1d76c1f32e0c711be93c3ecbf170c00acd2e6582/images/CNC/CNC2.jpeg" alt="Arduino-input" width="1400">

17. When the machine tool alarm occurs, the cause should be identified according to the alarm number and eliminated in time.
18. Regularly clean up the iron filings and other debris in the coolant box, and timely supplement the coolant according to the regulations.
19. Without the permission of the workshop supervisor, do not insert U (hard) disk, CD into the CNC machine tool, do not modify or delete the process in the machine tool
Order.
20. After work, clean up the site, clean the iron filings of CNC machine tools, wipe the lathe, oil anti-rust, according to the regulations in the refueling part of the oil, the workpiece on the shelf neatly placed, do 5S work.


Reference web:
1. https://www.tmt.com.tw/cht/news/precautions-for-safety-operation-of-cnc-lathe.html#:~:text=1.%20%E5%AE%89%E5%85%A8%E6%93%8D%E4%BD%9C%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A0%85,%E4%B8%8D%E5%8F%AF%E8%B6%85%E8%B2%A0%E8%8D%B7%E5%8A%A0%E5%B7%A5%E3%80%82
2. https://www.safehoo.com/Item/332371.aspx
3. https://zhidao.baidu.com/question/2122336893294112307.html