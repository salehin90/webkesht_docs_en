---
title:  WebKesht Smart Irrigation- A Quick Start Guide
description: In this comprehensive guide, learn step-by-step how to set up and make your first use of the WebKesht smart irrigation management system and get started.
---
<script>
// ایجاد overlay برای نمایش تمام صفحه
document.addEventListener('DOMContentLoaded', function() {
    // ایجاد المان overlay
    const overlay = document.createElement('div');
    overlay.className = 'image-fullscreen-overlay';
    overlay.innerHTML = '<div class="fullscreen-close-btn">✕</div>';
    document.body.appendChild(overlay);

    // انتخاب تمام تصاویر داخل image-container
    const images = document.querySelectorAll('.image-container img');
    
    images.forEach(img => {
        img.addEventListener('click', function(e) {
            e.stopPropagation();
            
            // ایجاد کپی از تصویر برای نمایش
            const clonedImg = this.cloneNode(true);
            clonedImg.style.cursor = 'zoom-out';
            
            // پاک کردن محتوای قبلی overlay
            const existingImg = overlay.querySelector('img');
            if (existingImg) {
                existingImg.remove();
            }
            
            // اضافه کردن تصویر جدید
            overlay.appendChild(clonedImg);
            overlay.classList.add('active');
            
            // غیرفعال کردن اسکرول
            document.body.style.overflow = 'hidden';
        });
    });
    
    // بستن overlay با کلیک روی پس‌زمینه یا دکمه بستن
    overlay.addEventListener('click', function() {
        closeFullscreen();
    });
    
    // بستن با کلید ESC
    document.addEventListener('keydown', function(e) {
        if (e.key === 'Escape' && overlay.classList.contains('active')) {
            closeFullscreen();
        }
    });
    
    function closeFullscreen() {
        overlay.classList.remove('active');
        document.body.style.overflow = 'auto';
        
        // حذف تصویر پس از انیمیشن
        setTimeout(() => {
            const img = overlay.querySelector('img:not(.fullscreen-close-btn)');
            if (img) img.remove();
        }, 300);
    }
});
</script>

<div class="container">

    <div class="header">
            <h1>🌱 WebKesht Smart Irrigation: A Quick Start Guide 💧</h1>
            <p>The Complete Guide to Using the WebKesht Smart Irrigation Management System - From Registration to Smart Irrigation</p>
    </div>

<div class="content">

            <p style="margin-bottom: 25px; text-align: justify; line-height: 1.8; font-size: 1.1em;"> Welcome to the WebKesht Smart Irrigation Management System. This guide will assist you through the process of registration, project creation, and defining essential parameters.</p>

</div>

<!-- بخش اول: ثبت‌نام و ورود -->
 
<div class="main-section" >
    <div class="section-header" onclick="toggleSection(this)"  >
                    <span> 👤 User Account: Registration and Login Guide</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify;"> To use the system’s features, you must first create a user account. </p>
                        <!-- زیربخش عضویت -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>📝 Signing Up for the System</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <div class="method-steps">
                                        <h4>📋 Steps to Complete:</h4>
                                        <div class="step-timeline">
                                            <div class="timeline-item">
                                                <strong>Step 1:</strong>
                                                  First, navigate to the at <strong>WebKesht website</strong>: 
												<a href="https://webkesht.com" target="_blank"><span class="message-code"> https://webkesht.com </span class="message-code"></a>
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 2:</strong> On the homepage, click the <strong>“Login / Sign In / Access Platform”</strong> button.
												<div class="image-container">
                                                <img src="images/01.home.JPG"  alt="Login to System">
                                            </div>
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 3:</strong> On the login page, select the <strong>“Sign-up”</strong> option
												<div class="image-container">
                                                <img src="images/02.signin.JPG" alt="Sign-up Page">
                                            </div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Step 4:</strong> Complete the registration form with the following information:
                                                <ul style="margin-top: 10px;">
												  <li><strong>Email:</strong> Enter a valid and unique email address. This email will be used as your username</li>
                                                    <li> <strong>Password:</strong> Choose a strong password with at least 6 characters, including uppercase and lowercase English letters, numbers, and symbols.</li>
												</ul>
                                            </div>
											<div class="timeline-item">
                                                <strong>Step 5:</strong>After completing the form, click the <strong>“Sign-up”</strong>  button
												<div class="image-container">
                                                 <img src="images/03.signinForm.JPG" alt="Sign-up Button">
                                            </div>
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 6: </strong> <span class="message-code">Registration accepted. Please check your email for further instructions</span>  message indicates that this step was successful. Now, check your email inbox
												<div class="image-container">
                                                 <img src="images/04.signinRegNote.JPG" alt="Success message ">
                                            </div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Step 7:</strong>In the email sent from WebKesht, click on the verification link <strong><span class="message-code">confirm your registration</span></strong> to activate your user account.
                                            <div class="image-container">
                                                 <img src="images/05.Email.JPG" alt="Verification Email">
                                            </div>
											</div>
											<div class="timeline-item">
                                                <strong>Step 8:</strong> After verification, you will be redirected to the login page, and a <span class="message-code">Your registration has been confirmed</span> will be displayed. Your registration is now complete.
												<div class="image-container">
                                                 <img src="images/06.EmailRegNote.JPG" alt="Final Confirmation Message">
                                            </div>
                                            </div>
                                        </div>
                                    </div>
								</div>
                         </div>            
                               </div>                             
                         <!-- زیربخش ورود -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🔑 Logging into the System </span>
                                <span class="sub-icon">−</span>
                            </div>
							<div class="sub-content">
							<div class="sub-body">
							<div class="timeline-item">
                                                <strong>Step 1:</strong>On the login page, enter the email (username) and password you set during registration.
                                                </div>
							<div class="timeline-item">
                                                <strong>Step 2:</strong> Click the <strong> Login </strong> button to be redirected to your user dashboard.
												<div class="image-container">
                                                <img src="images/07.LoginForm.JPG" alt="Login Page">
                                            </div>
                              </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <div class="note-box">
                                        <strong>📌 Important Dashboard Tips:</strong>
                                        <ul>
                                            <li>To switch the system theme between Light and Dark mode, click the <strong>Sun/Moon</strong> icon.</li>
                                            <li>To change your password or log out of your account, click the <strong>user profile icon</strong> .</li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
					</div>
                </div>
				</div>
                </div>
            <div class="separator"></div>
 <!-- بخش دوم: مدیریت پروژه‌ها -->
            <div class="main-section" >
                <div class="section-header" onclick="toggleSection(this)">
                    <span>📁 Project Management Guide</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify;"> Each project in WebKesht can represent a separate farm, orchard, or green space.</p>
                      <!-- زیربخش ایجاد پروژه -->
					  <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>➕ Creating a New Project </span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <div class="method-steps">
                                        <h4>📋 Steps to Complete:</h4>
                                        <div class="step-timeline">
											<div class="timeline-item">
                                                <strong>Step 1:</strong> After your first login, you will land on the “Projects List” page. To begin, click the <strong>“New”</strong> button.
												<div class="image-container">
													<img src="images/08.ProjectList.JPG" alt="Projects List">
													</div>
												</div>
											</div>
											<div class="timeline-item">
                                                <strong>Step 2:</strong>In the form that opens, enter the <strong>project name</strong> and a corresponding <strong>description.</strong>
											</div>
											<div class="timeline-item">
                                                <strong>Step 3:</strong>Click the <strong>“Save”</strong> button. Your new project will now appear in the “Projects List"
												<div class="image-container">
													<img src="images/09.CreateNewProject.JPG" alt="Create Project Form">
													</div>
												</div>
											</div>
                                    </div>
								</div>
                         </div>            
                        <!-- زیربخش کار با لیست -->
						<div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>📋 Working with the Projects List</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p>The projects list table displays the following information:</p>
                                    <div class="method-steps">
                                        <h4>📋 Steps to Complete:</h4>
                                        <div class="step-timeline">
											<div class="timeline-item">
                                                <strong>ID:</strong> The unique project code.
											</div>
											<div class="timeline-item">
                                                <strong>Project Name:</strong> he name you have chosen.
											</div>
											<div class="timeline-item">
                                                <strong>Status :</strong>Indicates if the project is Active or Inactive
											</div>
											<div class="timeline-item">
                                                <strong>Operations:</strong>
												<ul style="margin-top: 10px;">
												  <li><strong>View:</strong> Enter the project management page (map and settings)</li>
                                                    <li> <strong>Delete:</strong> Permanently deletes the project</li>
												</ul>
												 <div class="image-container">
													<img src="images/10.NewProjectList.JPG" alt="Projects Table">
												</div>
											</div>
											<div class="note-box">
                                        <strong>💡 Note:</strong>In large tables, you can use the <strong>“Search…”</strong> bar to quickly find items, change the number of items displayed per page, and navigate between pages.
                                        <div class="image-container" style="margin-top: 15px;">
                                            <img src="images/11.ProjectListSearch.JPG" alt="Table Search and Pagination Tools">
                                        </div>
                                    </div>
                                    </div>
								</div>
                            </div>            
                        </div>           
                 </div>       
                 </div>
                 </div>
				<div class="separator"></div>
            <!-- بخش سوم: پارامترهای پایه -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>⚙️ Guide to Defining Basic Project Parameters</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify;"> After creating a project, click <strong>“View”</strong> to enter its management environment. In the right-hand column, you will find tools for defining the physical characteristics of your project. For optimal irrigation management, you must first define the information related to the irrigation system, soil, and vegetation cover. (Note: When a project is created, a set of default basic parameters is provided, which you can also use).
                        </p>
                        <div class="image-container">
                            <img src="images/12.ProjectHome.JPG" alt="Project Management Environment">
                        </div>
                        <!-- زیربخش سیستم‌های آبیاری -->
						<div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>💧 Managing Irrigation Systems(Irrigation System List)</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p>In this section, you will define the types of irrigation systems used in your project.</p>
								<div class="highlight">
                                        <strong>📝  To add a new system:</strong> Click on <strong>“Add New Irrigation System”</strong> and complete the following form:
                                </div>
                                    <div class="method-steps">
                                        <div class="step-timeline">
											<div class="timeline-item">
                                                <strong>Irrigation System Name:</strong>8 LPH Dripper, PS10A Sprinkler 
											</div>
											<div class="timeline-item">
                                                <strong>Precipitation rate (mm/hr):</strong>The amount of water the system applies per unit of time and area.
											</div>
											<div class="timeline-item">
                                                <strong>Irrigation Efficiency (%):</strong> Specify the irrigation efficiency based on the system type..
											</div>
											<div class="timeline-item">
                                                <strong>Operations:</strong> You can <strong>Edit</strong>, <strong>Delete</strong>, or <strong>Duplicate (copy)</strong>existing systems
											</div>
											<div class="timeline-item">
                                                <strong>Export:</strong>You can export a list of defined systems in <strong>Excel</strong> or <strong>CSV</strong> format.</li>.
											</div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <div class="note-box">
                                        <strong>📌 Additional Guidance:</strong>
                                        <ul>
                                            <li></strong>For more information about irrigation system types, please refer to the User Guides > <a href="https://webkesht.com/user-guide/Irrigation/" target="_blank"><span> “Comprehensive Irrigation System Guide”</span class="message-code"></a> section. </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
											<div class="image-container">
													<img src="images/13.IrrigationList.JPG" alt="Managing Irrigation Systems Interface">
												</div>
                                    </div>
								</div>
                         </div>            
                    </div>           
                 </div>  
 						<!-- زیربخش انواع خاک -->
						<div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🌍 Soil Type Management (Soil Types List)</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p>In this section, you will define the different soil textures present in your project.</p>
								<div class="highlight">
                                        <strong>📝 Adding a New Soil Type:</strong>To add a new soil type: Click on <strong>“Add New Soil”</strong> and complete the following fields:
                                </div>
                                    <div class="method-steps">
                                        <div class="step-timeline">
											<div class="timeline-item">
                                                <strong>Name :</strong> The name of the soil texture. Example: Clay Loam, Sandy.
											</div>
											<div class="timeline-item">
                                                <strong>Final Infiltration Rate (m/h):</strong>The maximum rate at which water can penetrate the soil once it is saturated.
											</div>
											<div class="timeline-item">
                                                <strong>Wilting Point Moisture (%): </strong>The minimum soil moisture level at which a plant can no longer extract water and begins to wilt.
											</div>
											<div class="timeline-item">
                                                <strong>Field Capacity Moisture (%):</strong> The maximum amount of moisture the soil can hold against gravity after excess water has drained away.
											</div>
											<div class="timeline-item">
                                                <strong>Operations: </strong>You can <strong>Edit</strong>، <strong>Delete</strong> or <strong>Duplicate </strong> each soil type.
											</div>
                                 <div class="sub-content">
                                     <div class="sub-body">
                                    <div class="note-box">
                                        <strong>📌 Additional Guidance:</strong>
                                        <ul>
                                        <li></strong>For more information about different soil types, please refer to the User Guides > <a href="https://webkesht.com/user-guide/Irrigation/" target="_blank"><span> “Comprehensive Soil Texture Guide”</span class="message-code"></a> section. </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                            <div class="image-container">
													<img src="images/14.SoilList.JPG" alt="Soil Type Management Interface">
												</div>
                                    </div>
								</div>
                         </div>            
                    </div>           
                 </div>       
                        <!-- زیربخش پوشش گیاهی -->
						<div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🌿 Vegetation Cover Management</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p>In this section, you define the types of vegetation planted in your project.</p>
								<div class="highlight">
                                        <strong>📝 To add new vegetation:</strong> Click on <strong>“Create New Vegetation”</strong> and complete the following form:
                                </div>
                                    <div class="method-steps">
                                        <div class="step-timeline">
											<div class="timeline-item">
                                                <strong>Crop Coefficient (Kc):</strong>A coefficient that defines the water needs of a specific plant relative to a reference plant.
											</div>
											<div class="timeline-item">
                                                <strong>Density Coefficient:</strong>A coefficient used to adjust water requirements based on planting density.
											</div>
											<div class="timeline-item">
                                                <strong>Root Depth (cm):</strong> The effective root depth of the plant that is considered in irrigation calculations.
											</div>
											<div class="timeline-item">
                                                <strong>Operations:</strong></strong>You can <strong>Edit</strong>، <strong>Delete</strong> or <strong>Duplicate </strong> each vegetation  type.
											</div>
<div class="sub-content">
                                     <div class="sub-body">
                                    <div class="note-box">
                                        <strong>📌 Additional Guidance:</strong>
                                        <ul>
                                        <li></strong>For more information about vegetation and selecting the correct coefficients, please refer to the User Guides > <a href="https://webkesht.com/user-guide/Irrigation/" target="_blank"><span> “Comprehensive Vegetation Cover Guide”</span class="message-code"></a> section. </li>
                                        </ul>
                                        </ul>
                                    </div>
                                </div>
                            </div>
											<div class="image-container">
                                        <img src="images/15.Vegetationlist.JPG" alt="Vegetation Management Interface">
                                    </div>
                                    </div>
								</div>
                         </div>            
                    </div>           
                 </div> 
                    </div>
                </div>
            </div>
            <div class="separator"></div>
 <!-- بخش چهارم: تعریف واحدهای مدیریتی -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>🗺️ Guide to Defining Management Units on the Map</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify;"> After defining the basic parameters, the next step is to draw the management zones on the satellite map.</p>
<!--  زیربخش ایجاد زیرواحد -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🔷 Creating a New Sub-unit (Solenoid Valve Zone)</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p style="margin-bottom: 15px;">A sub-unit is a geographical area (polygon) that is irrigated by a single solenoid valve or an independent management unit.</p>
                                    <div class="method-steps">
                                        <h4>📋 Steps to Create a Sub-unit:</h4>
                                        <div class="step-timeline">
                                            <div class="timeline-item">
                                                <strong>Step 1:</strong>Click the <strong>“New Sub-unit”</strong> button. The mouse cursor will change, indicating it is ready for drawing.
                                            <div class="image-container">
                                                <img src="images/16.NewSubunit.JPG" alt="New Sub-unit button">
                                            </div>
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 2:</strong>Draw the desired zone by clicking successively on the map to create vertices. To close the polygon, click on the starting point.
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 3:</strong>After drawing the polygon, the sub-unit information form will appear. Complete the following fields:
												<ul style="margin-top: 10px;">
												<li><strong>Sub-unit Name:</strong>  A descriptive name (e.g., North Saffron Plot, Park Lawn).</li>
                                                <li><strong>Vegetation Type, Irrigation System, Soil Type:</strong> Select the appropriate option for this zone from the lists you defined in the previous steps.</li>
                                                <li><strong>Microclimate Coefficient:</strong> To fine-tune water requirements based on specific local conditions (such as slope, shade, etc.).</li>
												</ul>
                                                <div class="image-container">
                                                <img src="images/17.AddNewSubunit.JPG" alt="Sub-unit information form">
												</div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Step 4:</strong>Click  <strong>“Save”.</strong>
                                            </div>
									<div class="note-box">
                                    <h4>⚙️ Managing a Sub-unit:</h4>
										<div class="method-steps">	
												<div class="step-timeline">
												<p style="margin-top: 10px;">Clicking on a drawn sub-unit on the map will open a pop-up window with the following options:</p>
												<ul style="margin-top: 10px;">
												<li><strong>Basic Info:</strong>  Displays initial calculations such as <strong>irrigation interval</strong>, <strong>watering duration</strong>, and <strong>flow rate</strong>.</li>
												<li><strong>Edit:</strong> Change the basic information of the sub-unit.</li>
												<li><strong>Edit Geometry:</strong> Modify the geographical boundary of the drawn polygon.</li>
												<li><strong>Irrigation Management:</strong> Access advanced settings for the irrigation scheduling type.</li>
												<li><strong>Reports:</strong> View the history of irrigation events..</li>
												<li><strong>Delete:</strong> Permanently deletes the sub-unit.</li>
												</ul>
												</div>
										</div>
										<div class="image-container" style="margin-top: 15px;">
                                            <img src="images/18.SubunitManagement.JPG" alt="Sub-unit management pop-up window">
                                        </div>
									</div>
                                    </div>
								</div>
                         </div>
</div>
</div>
</div>
<!-- زیربخش افزودن دستگاه -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>📡 Adding a New Device (IoT Controller)</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
								<p style="margin-bottom: 15px;">The device is a controller panel that receives irrigation commands from the system and sends them to the solenoid valves.</p>
                                    <div class="method-steps">
                                        <h4>📋 Creation Steps:</h4>
                                        <div class="step-timeline">
                                            <div class="timeline-item">
                                                <strong>Step 1:</strong> Click the <strong>“New Device”</strong> button.
                                            <div class="image-container">
                                    <img src="images/16.NewSubunit.JPG" alt="IoT Device">
                                    </div>
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 2:</strong>Click on the map to mark the location where the device is installed.
                                            </div>
                                            <div class="timeline-item">
                                                <strong>Step 3:</strong>Complete the device information form:
												<ul style="margin-top: 10px;">
												<li><strong>Device Type:</strong> Select your controller device model from the list.</li>
                                                <li><strong>IoT Gateway ID, IoT Device ID, Ownership Token:</strong> This information is provided to you by the device supplier.</li>
												</ul>
                                                <div class="image-container">
                                                <img src="images/19.AddController.JPG" alt="Device information form">
                                            </div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Step 4:</strong>Click  <strong>“Save”.</strong> 
                                            </div>
											<div class="note-box">
											<div class="method-steps">	
											<h4>⚙️ Managing a Device:</h4>
												<div class="step-timeline">
												<p style="margin-top: 10px;">Clicking on the device icon on the map opens a pop-up window with the following options:</p>
												<ul style="margin-top: 10px;">
												<li><strong>حذف:</strong>  Deletes the device from the project</li>
												<li><strong>Manage Connections:</strong> This is a crucial section for connecting sub-units to the device.</li>
												</ul>
												</div>
											</div>
											<div class="image-container" style="margin-top: 15px;">
                                            <img src="images/20.EditController.JPG" alt="Device management">
											</div>
											</div>
										</div>
									</div>
								</div>            
							</div>  		
						</div>
<!-- زیربخش اتصال زیرواحد -->
                        <div class="sub-section">
                            <div class="sub-header" onclick="toggleSubSection(this)">
                                <span>🔗 Connecting a Sub-unit to a Device</span>
                                <span class="sub-icon">−</span>
                            </div>
                            <div class="sub-content">
                                <div class="sub-body">
                                    <ol class="step-list">
                                        <li>In the device management window, click on <strong>“Manage Connections”. </strong></li>
                                        <li>Select <strong>“Create New Output”</strong>.</li>
                                        <li>Select the desired sub-unit on the map.</li>
                                        <li>Once the sub-unit is added to the output list, a dashed line will appear on the map, visually connecting the device to the sub-unit.</li>
                                        <li>Repeat this process for all sub-units that are controlled by this device.</li>
                                    </ol>
                                    <div class="image-container" style="margin-top: 15px;">
                                            <img src="images/21.EditSubunit-Controller.JPG" alt="Managing Sub-unit Connections">
                                        </div>
                                    <div class="highlight">
                                        <strong>✅ Note:</strong>  After a successful connection, the dashed line linking the device and the sub-unit will be visible on the map.
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
   </div>    
<div class="separator"></div>
<!-- بخش پنجم: مدیریت هوشمند آبیاری -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>🤖 Guide to Smart Irrigation Management</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify;"> After defining the sub-units and connecting them to devices, you can specify the type of irrigation schedule. These settings are accessible via the <strong>“Irrigation Management”</strong> option in each sub-unit’s pop-up window.</p>
                        <div class="sub-content">
                                <div class="sub-body">
                                    <div class="method-steps">
                                        <h4>Types of Irrigation Schedules:</h4>
                                        <div class="step-timeline">
                                            <div class="timeline-item">
                                                <strong>Manual Irrigation:</strong> In this mode, the system only performs the calculations; the user is responsible for manually opening and closing the valves.
                                                <div class="image-container">
                                                <img src="images/22.ManualIrrigation.JPG" alt="Manual Irrigation Settings">
												</div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Automatic Irrigation:</strong> Irrigation is performed based on a fixed, pre-defined schedule, and the system automatically sends commands to the controller.                                                
                                                <div class="image-container">
                                                <img src="images/23.AutomaticIrrigation.JPG" alt="Automatic Irrigation Settings">
												</div>
                                            </div>
											<div class="timeline-item">
                                                <strong>Smart Irrigation (Recommended Option):</strong> In this mode, the system dynamically calculates the precise water requirement daily based on <strong>real-time online weather data </strong> (temperature, humidity, evapotranspiration) and the project’s specific parameters. The system then executes the irrigation schedule dynamically. Furthermore, the irrigation forecast for the next 7 days is calculated and available for viewing.
											<div class="image-container">
                                            <img src="images/24.SmartIrrigation.JPG" alt="Smart Irrigation Settings">
												</div>
                                            </div>
                                        </div>
                                    </div>
								</div>
                         </div>  
                        <div class="highlight" style="margin-top: 25px;"> By completing these steps, your project is now fully set up for smart irrigation management. The WebKesht system will automatically begin to optimize water consumption for your farm, garden, or green space.
                        </div>
                    </div>
                </div>
            </div>
        </div>
