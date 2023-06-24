# Design_and_analysis_of_nmos_pmos_and_Inverter_using_sky130pdk

Welcome to the Design and Analysis project using the SkyWater130 Process Design Kit (PDK). In this project, we will explore the characteristics and behavior of NMOS and PMOS devices, as well as design and analyze a CMOS inverter, utilizing the capabilities of the SkyWater 130nm process technology.

**Analysis of NMOS and PMOS**

We will begin by utilizing the 1.8V standard models of NMOS and PMOS available in the SkyWater130 PDK. Through analysis and experimentation, we will explore the common working principles of these devices and characterize their behavior by varying different parameters. This analysis will provide valuable insights into their performance and functionality.

**Design and Analysis of CMOS Inverter**

Next, we will dive into the design and analysis of a CMOS inverter. This will involve creating the schematic representation of the inverter and measuring various parameters such as delay, noise margin, rise time, and fall time. These measurements will serve as a case study to study SPICE simulation and understand the behavior of the CMOS inverter.

**Layout Design using MAGIC**

In the subsequent phase, we will shift our focus to the layout design of the CMOS inverter using the MAGIC layout editor. MAGIC provides a comprehensive platform for exploring and utilizing the different layers available in the SkyWater130 PDK. We will create the layout design of the inverter, ensuring adherence to design rules and constraints.

**Layout versus Schematic (LVS) Comparison**

To ensure the accuracy and consistency of our layout, we will perform a Layout versus Schematic (LVS) comparison. This step involves comparing the layout design with the previously created schematic representation. By utilizing tools like Netgen and the LVS capabilities of the SkyWater130 PDK, we will verify the correctness and integrity of the layout.

Throughout the project, we will leverage the models and resources provided by the SkyWater130 PDK, as well as open-source tools such as Xschem, NGSPICE, MAGIC, and Netgen. The project documentation will be structured in a manner that is easily understandable for anyone looking to follow the same methodology.

Join us in this exciting journey of designing and analyzing NMOS, PMOS, and CMOS circuits using the SkyWater130 PDK. Let's explore the capabilities of the PDK and gain valuable insights into the world of electronic design.

# Content

 **1. About Tools**
    
     1.1 Ngspice
    
     1.2 Magic
    
     1.3 Netgen
    
     1.4 xschem
    
     1.5 Skywater Technology
   
 3. Analysis of MOSFET models
   
     2.1 General MOS analysis
   
     2.2 strong 0 and weak
   
     2.3 Weak 0 and strong 1

 4. CMOS Inverter Design and Analysis
     3.1 Why CMOS Circuits
    
     3.2 CMOS Inverter Analysis(Pre-Layout)

  # 1. About Tools
  
   **1.1 Ngspice**
   
  ![image](https://github.com/SudeepGopavaram/Design_and_analysis_of_nmos_and_pmos_using_sky130pdk/assets/57873021/9073cdd0-8e57-4177-9557-cc476fa6e9c2)

  Ngspice is an open-source mixed-level/mixed-signal electronic circuit simulator widely used for circuit design, analysis, and verification. It allows users to 
  model and simulate the behavior of electronic circuits using a variety of circuit elements, including resistors, capacitors, inductors, transistors, and more.

  Ngspice provides a command-line interface for interaction and scripting, making it flexible and suitable for both interactive usage and automated workflows. It 
  supports a wide range of circuit netlist formats, including the popular SPICE format, allowing seamless integration with existing design flows and tools.

   Its versatility and accessibility make it a valuable asset in the field of electronic design automation.

   **1.2 Magic**
   
   ![image](https://github.com/SudeepGopavaram/Design_and_analysis_of_nmos_and_pmos_using_sky130pdk/assets/57873021/57ec58d6-9023-4d6a-ae0e-eb2db101f1db)

   Magic is an open-source layout tool widely used in the field of digital integrated circuit design. It provides a powerful platform for creating and editing 
   layouts of integrated circuits at various levels of abstraction, ranging from individual transistors to complete chip designs.
   
   Magic offers a range of features to enhance productivity and design efficiency. It includes a comprehensive set of drawing tools and alignment aids to facilitate 
   precise and accurate layout creation. It supports design rule checking (DRC) and layout versus schematic (LVS) verification, helping to identify and resolve 
   potential design errors and mismatches.

   Its feature-rich nature, extensibility, and community support make it an invaluable asset in the realm of digital integrated circuit design.

   **1.3 Netgen**
   
   ![image](https://github.com/SudeepGopavaram/Design_and_analysis_of_nmos_and_pmos_using_sky130pdk/assets/57873021/215efd81-b834-4845-a390-d8c8be694ed2)

   Netgen is an open-source netlist comparison and verification tool used in the field of electronic design automation (EDA). It provides a powerful platform for 
   analyzing and comparing digital circuit netlists to ensure consistency and correctness across different stages of the design process.

   Netgen supports a wide range of netlist formats, including popular industry standards like SPICE and Verilog. It offers comprehensive netlist parsing and analysis 
   capabilities, allowing you to explore the hierarchical structure of the design, examine signal dependencies, and identify potential issues.

   Its ability to detect discrepancies and ensure design consistency contributes to the overall success and reliability of your circuit designs.

   **1.4 Xschem**
   
   ![image](https://github.com/SudeepGopavaram/Design_and_analysis_of_nmos_and_pmos_using_sky130pdk/assets/57873021/90b859e9-d0f5-4bca-bff5-cb439948ecec)

   Xschem is an open-source electronic schematic capture and simulation tool widely used in the field of electronic design automation (EDA). It provides a versatile 
   platform for designing and simulating analog and digital circuits, facilitating the creation and analysis of complex circuit schematics.

   Xschem also supports advanced features such as model parameter extraction, sensitivity analysis, and waveform plotting, allowing you to fine-tune circuit designs 
   and explore design trade-offs. It offers a flexible scripting interface, enabling automation of repetitive tasks and customization of the tool's behavior to suit 
   specific requirements.

   Its user-friendly interface, extensive simulation capabilities, and community support make it an invaluable tool in the field of electronic design.

   **1.5 Skywater Technology**
   
   ![image](https://github.com/SudeepGopavaram/Design_and_analysis_of_nmos_and_pmos_using_sky130pdk/assets/57873021/f8f19c5c-1ded-40c1-a87b-82dc2e572bab)

   The SkyWater Technology Foundry 130nm Process Design Kit (PDK) is a comprehensive collection of files, libraries, and documentation that enables the design and 
   fabrication of integrated circuits (ICs) using the SkyWater 130nm process technology.

   The SkyWater130 PDK is typically utilized in conjunction with electronic design automation (EDA) tools, enabling designers to create and verify their IC designs 
   within a familiar design environment. The PDK provides the necessary information for layout design, including design rules, layer information, and guidelines for 
   ensuring compatibility with the SkyWater 130nm process technology.

   Overall, the SkyWater130 PDK is an essential resource for IC designers seeking to leverage the capabilities of the SkyWater 130nm process technology. Its 
   comprehensive set of files, libraries, and guidelines streamline the design process and facilitate the creation of high-quality integrated circuits.

   

   
   
     
     
