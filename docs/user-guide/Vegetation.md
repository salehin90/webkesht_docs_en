---
title: A Comprehensive Guide to Defining Vegetation Types in WebKesht
description: Introduction to Essential Vegetation Parameters for the WebKesht Smart Irrigation System
---

   <div class="container">
        <div class="header">
             <h1> A Guide to Determining Vegetation Parameters for Smart Management 🌱</h1>

        </div>

        <div class="content">
            <p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> Optimal irrigation and water waste prevention require a precise understanding of your plants’ water needs. The three primary parameters our irrigation algorithms need to calculate the actual water consumption of the plants are: <strong>Species Factor</strong>, <strong>Density Coefficient</strong> and <strong>Root Depth</strong>. </p>
<p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> For the software to perform calculations accurately, you must group your vegetation based on <strong>irrigation sub-units</strong> (any area irrigated by <strong> a separate valve</strong>) and define the above parameters for each group. </p>


<p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> 
<strong>How to Create This List? </strong> </p>
<p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> The fundamental and key rule for defining vegetation in the software is this:
<strong>The list of vegetation types is determined based on the water needs and shared management of irrigation sub-units (separate valves).</strong></p>

 <p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> 
In practice, for each <strong>irrigation sub-unit</strong>, you specify its vegetation type. If several sub-units (multiple valves) have a <strong>common</strong> or <strong>similar vegetation</strong> type in terms of water needs, you only need to define that vegetation type <strong>once</strong> in the software.

</p>
<p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> <strong> Examples: </strong> </p>


 <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Scenario </th>
                                        <th>Irrigation Sub-units (Separate Valves)</th>
                                        <th>Vegetation Type in the Sub-unit</th>
                                        <th>How to Define in the Vegetation List</th>
                                        <th>Decision Logic</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><strong> Example 1: Green Space</strong></td>
                                        <td>Sub-unit 1: Turf (Sprinkler) </br>
                                            Sub-unit 2: Seasonal Flowers</br>
                                            Sub-unit 3: Trees (Subsurface) </td>
                                        <td>Turf, Seasonal Flowers, Trees</td>
                                        <td>3 Vegetation Types:</br>
                                            Turf</br>
                                            Flowers</br>
                                            Trees</td>
                                        <td>Each sub-unit has a completely different vegetation type and water requirement, so they must have their own specific parameters defined. </td>     
                                    </tr>
                                    <tr>
                                        <td><strong>Example 2: Large Orchard</strong></td>
                                        <td>10 separate sub-units (the entire orchard)</td>
                                        <td>Mixed fruit trees (Apple, Plum, Apricot)</td>
                                        <td>br><br> 1 Vegetation Type: <br> Mixed Fruit Trees </td>
                                        <td> Despite having 10 separate valves, because the vegetation is similar across all sub-units and has the same water requirement, defining a single vegetation type is sufficient. </td> 
                                    </tr>   
                                </tbody>
                            </table>

                            
                        </div>
<p style="margin-bottom: 25px; text-align: justify; line-height: 1.8;"> In the following sections, you will find a step-by-step guide to accurately determine the Species Factor, Density Coefficient, and Root Depth to complete this section. </p>



            <!-- بخش 1: فاکتور گونه -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>🌿 Species Factor (Species Factor)</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content ">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> The species factor is determined based on the species’ water requirement, independent of environmental conditions and other factors. This factor indicates how much more (or less) water your plant needs compared to a standard reference (such as turfgrass). </p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">📊 Range of Variation for the Species Factor:</h4>
                        
                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th> Species Factor Based on Water Need</th>
                                        <th>Species Factor Value</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><strong>Very Low</strong></td>
                                        <td>Less than 0.1</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Low</strong></td>
                                        <td>0.1 - 0.3</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Medium</strong></td>
                                        <td>0.4 - 0.6</td>
                                    </tr>
                                    <tr>
                                        <td><strong>High</strong></td>
                                        <td>0.7 - 0.9</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>

                        <div class="note-box">
                            <strong>📌 Note:</strong>In the plant species characteristics table, the species factor is provided for several green space species. In this table, <strong>“H”</strong> indicates a high-need plant species, <strong>“M”</strong> indicates a medium water-need species, and <strong>“L”</strong> indicates a low-need species.
                            
                        </div>
                    </div>
                </div>
            </div>

            <div class="separator"></div>

            <!-- بخش 2: ضریب تراکم -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>📐 Plant Density Factor </span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content ">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> The density of plants in a green space varies due to differences in plant maturity stages and the spacing between diverse plant species. Medium density is a condition where, similar to turfgrass, the cultivated area is 90% to 100% covered. As coverage decreases from this amount, the density coefficient can be reduced to as low as 0.5.</p>

                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;">Density coefficient values greater than one are applicable when a double canopy is created due to the mixed cultivation of groundcover plants and other plants alongside each other, such as planting trees and shrubs in layered arrangements within a turf-covered area. </p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">📊 Range of Density Coefficient for Plants Used in Green Spaces:</h4>
                        
                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Species Need</th>
                                        <th>Coefficient Value</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><strong>Low Density</strong></td>
                                        <td>0.5 - 0.9</td>
                                    </tr>
                                    <tr>
                                        <td><strong>Medium Density</strong></td>
                                        <td>1</td>
                                    </tr>
                                    <tr>
                                        <td><strong>High Density</strong></td>
                                        <td>1.1 - 1.3</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>

                    </div>
                </div>
            </div>

            <div class="separator"></div>

            <!-- بخش 3: عمق ریشه -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>🌳 Root Depth</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content ">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> Root depth determines how deep water must penetrate the soil to become available to the plant’s active roots. Root depth depends on the plant’s age, type (tree, shrub, or turf), and soil conditions (such as the presence of restrictive layers or the depth of the water table).</p>

                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> In the Plant Species Characteristics Table, root depth is presented descriptively based on the root system type of green space plant species.</p>

                        <h4 style="margin: 20px 0 15px 0; color: #2c3e50; font-size: 1.05em;">📏  Usage Guide:</h4>
                        <p style="margin-bottom: 15px; text-align: justify; line-height: 1.8;"> Enter the root depth in centimeters for your system:</p>

                        <div class="definition-grid">
                            <div class="definition-card">
                                <h3>🌱 Shallow</h3>
                                <p><strong>Range:</strong> 10 - 40 cm</p>
                                <p>Suitable for groundcovers and turf</p>
                            </div>

                            <div class="definition-card">
                                <h3>🌿 Medium</h3>
                                <p><strong>Range:</strong> 40 - 70 cm</p>
                                <p> Suitable for shrubs and small trees</p>
                            </div>

                            <div class="definition-card">
                                <h3>🌳 Deep</h3>
                                <p><strong>Range:</strong> 70 - 150+ cm</p>
                                <p> Suitable for large trees</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="separator"></div>

            <!-- بخش 4: جدول مشخصات گونه‌های گیاهی -->
            <div class="main-section">
                <div class="section-header" onclick="toggleSection(this)">
                    <span>📋 Plant Species Characteristics Table</span>
                    <span class="section-icon">−</span>
                </div>
                <div class="section-content ">
                    <div class="section-body">
                        <p style="margin-bottom: 20px; text-align: justify; line-height: 1.8;"> The table below provides complete information on the water needs and root depth for 64 common plant species used in green spaces:</p>

                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Row</th>
                                        <th>Name</th>
                                        <th>Scientific Name</th>
                                        <th>Water Need</th>
                                        <th>Root Depth (Descriptive)</th>
                                    </tr>
                                </thead>
                                <tbody>
                                <tr>
                                        <td>1</td>
                                        <td>aluminium plant</td>
                                        <td>Pilea cadierei</td>
                                        <td>M</td>
                                        <td>Shallow; groundcover plant.</td>
                                    </tr>
                                <tr>
                                        <td>2</td>
                                        <td>Bentgrass</td>
                                        <td>Agrostis stolonifera</td>
                                        <td>M</td>
                                        <td>Shallow (subsurface); dense and fibrous root system (10 to 30 cm depth)</td>
                                    </tr>
                                <tr>
                                        <td>3</td>
                                        <td>Bird of paradise</td>
                                        <td>Erythrostemon gilliesii</td>
                                        <td>L</td>
                                        <td>Medium to Deep; for water absorption in dry conditions.</td>
                                    </tr>
                                <tr>
                                        <td>4</td>
                                        <td>Black pine</td>
                                        <td>Pinus nigra</td>
                                        <td>L</td>
                                        <td>Deep; strong and extensive roots.</td>
                                    </tr>
                                <tr>
                                        <td>5</td>
                                        <td>Bukhara fleeceflower</td>
                                        <td>Fallopia baldschuanica</td>
                                        <td>M</td>
                                        <td>Medium; fast growing and clump forming root.</td>
                                    </tr>
                                <tr>
                                        <td>6</td>
                                        <td>Carex </td>
                                        <td>Carex humilis</td>
                                        <td>H</td>
                                        <td>Shallow; herbaceous plant with fibrous roots.</td>
                                    </tr>
                                <tr>
                                        <td>7</td>
                                        <td>Caspian locust</td>
                                        <td>Gleditsia caspica</td>
                                        <td>L</td>
                                        <td>Deep; main roots for establishment.</td>
                                    </tr>
                                <tr>
                                        <td>8</td>
                                        <td>Chinaberry tree</td>
                                        <td>Melia azedarach</td>
                                        <td>L</td>
                                        <td>Deep and extensive; can damage infrastructure.</td>
                                    </tr> 
                                <tr>
                                        <td>9</td>
                                        <td>Chinese fountain grass</td>
                                        <td>Pennisetum alopecuroides</td>
                                        <td>L</td>
                                        <td>Medium to Deep; well-developed and drought-resistant root system.</td>
                                    </tr> 
                                <tr>
                                        <td>10</td>
                                        <td>Chinese wisteria</td>
                                        <td>Wisteria sinensis</td>
                                        <td>M</td>
                                        <td>Deep; strong and woody root, requires ample space.</td>
                                    </tr>
                                <tr>
                                        <td>11</td>
                                        <td>Common Hibiscus</td>
                                        <td>Hibiscus syriacus</td>
                                        <td>M</td>
                                        <td>Medium; dense and clump-forming root.</td>
                                    </tr>
                                <tr>
                                        <td>12</td>
                                        <td>Coneflowers</td>
                                        <td>Rudbeckia hirta</td>
                                        <td>M</td>
                                        <td>Taproot; thick and deep main root.</td>
                                    </tr>
                                <tr>
                                        <td>13</td>
                                        <td>Corn Plant</td>
                                        <td>Dracaena compacta</td>
                                        <td>M</td>
                                        <td>Shallow and clump-forming; usually grown as a potted plant.</td>
                                    </tr>
                                <tr>
                                        <td>14</td>
                                        <td>Cotoneaster</td>
                                        <td>Cotoneaster horizentaliss</td>
                                        <td>L</td>
                                        <td>Shallow; small and fibrous roots.</td>
                                    </tr>
                                <tr>
                                        <td>15</td>
                                        <td>Crape myrtle</td>
                                        <td>Lagerstroemia indica</td>
                                        <td>H</td>
                                        <td>Shallow; it’s best for the upper roots to be near the soil surface.</td>
                                    </tr>
                                <tr>
                                        <td>16</td>
                                        <td>Dog rose</td>
                                        <td>Rosa canina</td>
                                        <td>M</td>
                                        <td>Medium to Deep; strong and clump-forming roots.</td>
                                    </tr>
                                <tr>
                                        <td>17</td>
                                        <td>Elm</td>
                                        <td>Ulmus boissieri</td>
                                        <td>M</td>
                                        <td>Deep with large surface roots; surface roots can lift sidewalks.</td>
                                    </tr>
                                <tr>
                                        <td>18</td>
                                        <td>Firethorns</td>
                                        <td>Pyracantha coccinea</td>
                                        <td>M</td>
                                        <td>Medium; fibrous and dense roots.</td>
                                    </tr>  
                                <tr>
                                        <td>19</td>
                                        <td>Florist's daisy</td>
                                        <td>Chrysanthemum morifolium</td>
                                        <td>M</td>
                                        <td>Shallow; clump forming and fibrous root.</td>
                                    </tr>   
                                <tr>
                                        <td>20</td>
                                        <td>Frankenia</td>
                                        <td>Frankenia thymofolia</td>
                                        <td>M</td>
                                        <td>Medium; fibrous roots.</td>
                                    </tr>                       
                                <tr>
                                        <td>21</td>
                                        <td>French tamarisk</td>
                                        <td>Tamarix gallica</td>
                                        <td>L</td>
                                        <td>Very Deep (invasive); capable of rooting to very great depths (over 4.5 meters).</td>
                                    </tr>
                                <tr>
                                        <td>22</td>
                                        <td>German iris</td>
                                        <td>Iris germanica</td>
                                        <td>M</td>
                                        <td>Rhizomatous (very shallow); rhizomes should be planted at or just below the soil surface.</td>
                                    </tr>
                                <tr>
                                        <td>23</td>
                                        <td>Golden Euonymus</td>
                                        <td>Euonymus japonica Aureo Marginata</td>
                                        <td>M-H</td>
                                        <td>Medium; dense and clump forming root.</td>
                                    </tr>
                                <tr>
                                        <td>24</td>
                                        <td>Golden rain tree</td>
                                        <td>Koelruteria paniculata</td>
                                        <td>H</td>
                                        <td>Deep and wide; for stability and moisture absorption.</td>
                                    </tr>
                                <tr>
                                        <td>25</td>
                                        <td>Hackberry</td>
                                        <td>Celtis australis - C.occidentalis</td>
                                        <td>L</td>
                                        <td>Deep; for high water absorption and stability.</td>
                                    </tr>
                                <tr>
                                        <td>26</td>
                                        <td>Holly oak</td>
                                        <td>Quercus ilex</td>
                                        <td>L</td>
                                        <td>Deep and extensive; for strength and stability.</td>
                                    </tr>
                                <tr>
                                        <td>27</td>
                                        <td>Hollyhocks</td>
                                        <td>Alcea sp</td>
                                        <td>M</td>
                                        <td>Taproot; thick and deep main root.</td>
                                    </tr>
                                <tr>
                                        <td>28</td>
                                        <td>Indian Shot</td>
                                        <td>Canna indica</td>
                                        <td>M</td>
                                        <td>Rhizomatous (underground); shallow and fibrous root system.</td>
                                    </tr>
                                <tr>
                                        <td>29</td>
                                        <td>Italian woodbine</td>
                                        <td>Lonicera caprifolium</td>
                                        <td>M</td>
                                        <td>Medium to Deep; strong roots to support climbing.</td>
                                    </tr>
                                <tr>
                                        <td>30</td>
                                        <td>Japanese barberry</td>
                                        <td>Berberis thunbergii</td>
                                        <td>M</td>
                                        <td>Shallow to Medium; fibrous and dense roots.</td>
                                    </tr>
                                <tr>
                                        <td>31</td>
                                        <td>Judas tree</td>
                                        <td>Cercis siliquastrum</td>
                                        <td>L</td>
                                        <td>Deep; strong and drought-resistant root system.</td>
                                    </tr>
                                <tr>
                                        <td>32</td>
                                        <td>Juniper</td>
                                        <td>Juniperus horizentalis</td>
                                        <td>L</td>
                                        <td>Shallow to Medium; extensive root system.</td>
                                    </tr>
                                <tr>
                                        <td>33</td>
                                        <td>Lady Banks' rose</td>
                                        <td>Rosa banksiae</td>
                                        <td>M</td>
                                        <td>Medium to Deep; strong and extensive root system.</td>
                                    </tr>
                                <tr>
                                        <td>34</td>
                                        <td>Lavender</td>
                                        <td>Lavandula angustifolia</td>
                                        <td>L-M</td>
                                        <td>Taproot; main root for stability.</td>
                                    </tr>
                                <tr>
                                        <td>35</td>
                                        <td>lucky plant</td>
                                        <td>Crassula ovata</td>
                                        <td>L</td>
                                        <td>Very Shallow; fibrous and shallow roots (succulent).</td>
                                    </tr>
                                <tr>
                                        <td>36</td>
                                        <td>Marguerite daisy</td>
                                        <td>Argyranthemum frutescens</td>
                                        <td>M</td>
                                        <td>Shallow; clump forming and fibrous root.</td>
                                    </tr>
                                <tr>
                                        <td>37</td>
                                        <td>Mediterranean cypress</td>
                                        <td>Cupressus sempervirens</td>
                                        <td>M</td>
                                        <td>Deep, extensive, and drought-resistant.</td>
                                    </tr>
                                <tr>
                                        <td>38</td>
                                        <td>Mountain pine</td>
                                        <td>Pinus mugo</td>
                                        <td>L</td>
                                        <td>Medium to Deep; strong root.</td>
                                    </tr>
                                <tr>
                                        <td>39</td>
                                        <td>New Zealand flax</td>
                                        <td>Phormium tenax</td>
                                        <td>L-M</td>
                                        <td>Fibrous and relatively shallow; dense and clump-forming root.</td>
                                    </tr>
                                <tr>
                                        <td>40</td>
                                        <td>Olive</td>
                                        <td>Olea europaea</td>
                                        <td>L</td>
                                        <td>Deep and extensive; for water absorption in dry Mediterranean conditions.</td>
                                    </tr>
                                <tr>
                                        <td>41</td>
                                        <td>Pampas grass</td>
                                        <td>Cortaderia selloana</td>
                                        <td>M</td>
                                        <td>Deep and dense; strong and clump-forming root system.</td>
                                    </tr>
                                <tr>
                                        <td>42</td>
                                        <td>Paper Mulberry</td>
                                        <td>Broussonetia papyrifera</td>
                                        <td>M-H</td>
                                        <td>Deep and extensive; similar to large trees.</td>
                                    </tr>
                                <tr>
                                        <td>43</td>
                                        <td>Pigface</td>
                                        <td>Carpobrotus edulis</td>
                                        <td>L</td>
                                        <td>Shallow; groundcover plant, superficial and creeping roots.</td>
                                    </tr>
                                <tr>
                                        <td>44</td>
                                        <td>pinkladies</td>
                                        <td>Oenothera speciosa</td>
                                        <td>M</td>
                                        <td>Taproot; main and deep root.</td>
                                    </tr>
                                <tr>
                                        <td>45</td>
                                        <td>Red hot pokers</td>
                                        <td>Kniphofia uvaria</td>
                                        <td>M</td>
                                        <td>Medium; fleshy and fibrous roots.</td>
                                    </tr>
                                <tr>
                                        <td>46</td>
                                        <td>Rosemary</td>
                                        <td>Salvia rosmarinus</td>
                                        <td>L-M</td>
                                        <td>Medium; strong and fibrous root.</td>
                                    </tr>
                                <tr>
                                        <td>47</td>
                                        <td>Russian olive</td>
                                        <td>Elaeagnus angustifolia</td>
                                        <td>L-M</td>
                                        <td>Deep and extensive; resistant to drought and salinity.</td>
                                    </tr>
                                <tr>
                                        <td>48</td>
                                        <td>Santolina</td>
                                        <td>Santolina virens</td>
                                        <td>L-M</td>
                                        <td>Shallow to Medium; fibrous roots.</td>
                                    </tr>
                                <tr>
                                        <td>49</td>
                                        <td>Silk tree</td>
                                        <td>Albizia julibrissin</td>
                                        <td>M</td>
                                        <td>Medium; extensive and dense roots.</td>
                                    </tr>
                                <tr>
                                        <td>50</td>
                                        <td>Silver ragwort</td>
                                        <td>Jacobaea maritima</td>
                                        <td>M</td>
                                        <td>Shallow; fibrous roots, suitable for ground cover.</td>
                                    </tr>
                                <tr>
                                        <td>51</td>
                                        <td>Steppegrass</td>
                                        <td>Stipa capansis</td>
                                        <td>L</td>
                                        <td>Medium to Deep; fibrous and drought resistant roots.</td>
                                    </tr>
                                <tr>
                                        <td>52</td>
                                        <td>Thuja</td>
                                        <td>Thuja orientalis</td>
                                        <td>M</td>
                                        <td>Shallow to Medium; extensive and dense roots.</td>
                                    </tr>
                                <tr>
                                        <td>53</td>
                                        <td>Trumpet vine</td>
                                        <td>Campsis grandiflora</td>
                                        <td>L-M</td>
                                        <td>Deep; strong and sometimes aggressive roots.</td>
                                    </tr>
                                <tr>
                                        <td>54</td>
                                        <td>Turkish pine</td>
                                        <td>Pinus brutia</td>
                                        <td>L</td>
                                        <td>Deep; strong roots for anchoring in rocky soils.</td>
                                    </tr>
                                <tr>
                                        <td>55</td>
                                        <td>wavyleaf sea lavender</td>
                                        <td>Limonium sinuatum</td>
                                        <td>M</td>
                                        <td>Medium; clump forming root.</td>
                                    </tr>
                                <tr>
                                        <td>56</td>
                                        <td>Waxleaf privet</td>
                                        <td>Ligustrum texanum-L.luccidum</td>
                                        <td>M-H</td>
                                        <td>Medium; strong and clump forming root.</td>
                                    </tr>
                                <tr>
                                        <td>60</td>
                                        <td>yarrow</td>
                                        <td>Achillea millefolium</td>
                                        <td>M</td>
                                        <td>Shallow and fibrous; the plant spreads via rhizomes.</td>
                                    </tr>
                                <tr>
                                        <td>57</td>
                                        <td>Yucca</td>
                                        <td>Yucca filamentosa</td>
                                        <td>L</td>
                                        <td>Medium to Deep; fleshy roots for water storage.</td>
                                    </tr>
                                    
                                    
                                </tbody>
                            </table>
                        </div>

                    
                    </div>
                </div>
            </div>

        </div>
    </div>

   