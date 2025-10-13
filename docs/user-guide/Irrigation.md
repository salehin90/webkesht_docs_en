---
title: A Comprehensive Guide to Defining Irrigation Systems in WebKesht
description: Defining irrigation systems and their essential parameters for the WebKesht smart irrigation system.
---

<div class="container">
        <div class="header">
            <h1> A Guide to Defining Irrigation Systems for Smart Irrigation Management💧</h1>
        </div>

        <div class="content">
            <p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;">
To enable the system to precisely set the irrigation duration and amount, it is essential to define the technical information of the irrigation systems used in your green space, garden, or farm. </p>

The goal of this section is for you to define the different systems that deliver water to the plants (such as sprinkler, drip, or subsurface), along with two key parameters: <strong>Efficiency</strong> and <strong>Precipitation Rate</strong>.
         
            <!-- بخش 1: راندمان سیستم آبیاری -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>⚙️ System Efficiency (Efficiency)</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">💧 What is Efficiency?</h4>
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> Efficiency indicates what percentage of the water distributed by the system is <strong>effectively stored in the plant’s root zone </strong> and is not lost (due to evaporation, wind drift, or runoff).                         </p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">⚡ The Importance of Efficiency </h4>
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> In its calculations, the system uses this number <strong>to compensate for water loss</strong>. The higher the system efficiency, the lower the water loss and the greater the irrigation productivity. </p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">📊 Efficiency Ranges for Different Irrigation Systems </h4>

                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Irrigation System Type</th>
                                        <th>Efficiency (%)</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><strong>Drip Irrigation</strong></td>
                                        <td>85-95 (Typically  90)</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Sprinkler Irrigation</strong></td>
                                        <td>70-85 (Typically  75)</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Flood / Furrow Irrigation</strong></td>
                                        <td>50-70 (Typically  60)</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Subsurface Irrigation</strong></td>
                                        <td>90-95</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>

                        <div class="note-box">
                            <strong>📌 Note: </strong>If available, use the measured or recommended values provided by the system’s manufacturer or designer.
                        </div>
                    </div>
                </div>
            </div>

            <div class="separator"></div>

            <!-- بخش 2: شدت پخش -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>💦 Precipitation Rate </span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">🔍 What is Precipitation Rate?</h4>
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> The precipitation Rate is <strong>the speed</strong> at which water is delivered to the soil by the irrigation system. This parameter is expressed in <strong> millimeters per hour (mm/hr)</strong>. </p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">⚡ The Importance of Precipitation Rate </h4>
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> This number determines how quickly water reaches the ground and directly impacts <strong>the irrigation duration</strong>. The software uses this parameter to precisely calculate how many minutes the valve must remain open to supply the required amount of water. </p>

                        <!-- زیربخش 1: آبیاری بارانی -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🌧️ How to Calculate for Sprinkler Irrigation</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <p style="margin-bottom: 18px; text-align: justify; line-height: 1.8;"> To calculate the Precipitation Rate for sprinkler systems, use the following formula:</p>
                                    <div class="formula-box">

                                        📊 Precipitation Rate $(mm/hr)$= Total Water Output $(l/h)$ $\div$ Covered Area $(m^2)$
                                    </div>
                                    <p style="margin-bottom: 18px; text-align: justify; line-height: 1.8;"> For a simple calculation, you can sum the output of all nozzles within a sub-unit and divide it by the total area of that sub-unit.</p>

                                    <h4 style="margin: 20px 0 12px 0; color: #2c3e50;">💡 Practical Example:</h4>
                                    <p style="text-align: justify; margin-bottom: 18px; line-height: 1.8;">
                                    If the total output of the nozzles is <strong> 400 liters per hour </strong> and the sub-unit area is liters per hour and the sub-unit area is <strong> 100 square meters </strong>:</p>

                                    <div class="formula-ex">
                                    Precipitation Rate = 400 $\div$ 100= 4 $(mm/hr)$  
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- زیربخش 2: آبیاری قطره‌ای -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>💧 How to Calculate for Drip Irrigation</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <p style="margin-bottom: 18px; text-align: justify; line-height: 1.8;"> To calculate the approximate Precipitation Rate for drip systems:</p>

                                    <div class="formula-box">
                                    📊 Approximate Precipitation Rate $(mm/hr)$= Emitter Flow Rate $(l/h)$ $\div$ Area per Emitter $(m^2)$
                                    </div>

                                    <h4 style="margin: 20px 0 12px 0; color: #2c3e50;">💡 Practical Example:</h4>
                                    <p style="text-align: justify; margin-bottom: 10px; line-height: 1.8;">
                                        Assume
                                    </p>
                                    <ul style="margin: 10px 0 18px 25px; line-height: 1.8;">
                                        <li>Emitter Flow Rate: <strong>4 Liters/hour</strong></li>
                                        <li>Spacing between emitters: <strong>1 meter</strong></li>
                                        <li>Spacing between rows (laterals): <strong>1 meter</strong></li>
                                        <li>
                                        Area per emitter= 1 $\div$ 1= 1 $(m^2)$</li>
                                    </ul>

                                    <div class="formula-ex">
                                    Precipitation Rate = 4 $\div$ 1= 4$(mm/hr)$
                                        </br>    
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div class="note-box" style="margin-top: 20px;">
                            <strong>📚 Important Note:</strong> If you have access to the catalog or technical manual for the emitters you are using (such as sprinklers or drippers), you can directly enter the application rate specified by the manufacturer.
                        </div>
                    </div>
                </div>
            </div>

            <div class="separator"></div>

            <!-- بخش 3: جمع‌بندی -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>✅ Summary and Usage Guide</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <div class="highlight">
                            <h4 style="margin: 0 0 15px 0; color: #2c5f2d;">🎯 By accurately defining these two key parameters, the system will be able to:</h4>
                            <ul style="margin: 10px 0 0 25px; line-height: 1.9;">
                                <li>Calculate the precise amount of water required.</li>
                                <li>Correctly determine the irrigation duration.</li>
                                <li>Minimize water loss.</li>
                                <li>Optimize irrigation productivity.</li>
                            </ul>
                        </div>

                        <p style="margin-top: 25px; text-align: justify; line-height: 1.8;"> For best results, it is recommended to use the detailed technical information for your irrigation system and, if possible, consult with irrigation specialists.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>



