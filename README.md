# 🏙️ Airbnb Bangkok Insights (วิเคราะห์ตลาดและผลกระทบของที่พักให้เช่าระยะสั้นในกรุงเทพฯ)

This project is an end-to-end data analysis project exploring the dynamics and impacts of short-term rental listings on Airbnb in Bangkok, Thailand. This project aims to deliver actionable insights through data visualizations and in-depth analysis to support stakeholders in decision-making.

## 👥 Authors

- **Pinthucha Ruckpintuwat**  
  `ID 65102010421` `pinthucharuckpintuwat@gmail.com`

## 🔗 Project Resources

- 📄 [Project Canvas](https://www.canva.com/design/DAGmXjOI3l0/ziHAPmuQZ_6Li6dkWGW9RQ/edit?utm_content=DAGmXjOI3l0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- 🧮 [Data Preparation Notebook (Colab)](https://colab.research.google.com/drive/1-02Nbqbo4TElalLMlemI1xjEYGpQB7U3?usp=sharing)
- 🔍 [Exploratory Data Analysis, EDA (Tableau)](#-exploratory-data-analysis-eda)
- 💡 [In-Depth Analysis (Tableau)](#-airbnb-bangkok-insights--in-depth-analysis)
- 📈 [Insights & Recommendations](#-airbnb-bangkok-insights--insights--recommendations)
- 📊 [Visualization (Tableau)](#-airbnb-bangkok--visualization--interactive-dashboard)
- 🎥 [Video Presentation](https://youtu.be/homWa8KuH88)

## 📌 Project Objectives

- Analyze how room types, location, and rental styles affect listing prices.
- Evaluate spatial distribution of listings to understand demand and supply across Bangkok.
- Assess the potential impact of Entire Homes and Long-term Listings on local housing availability.
- Use price, review scores, and listing types to recommend sustainable pricing strategies.

## 📊 Tools & Technologies

- **Data**: `listings.csv` from Inside Airbnb  
- **Languages**: Python (pandas, matplotlib)  
- **Platforms**: Google Colab, Tableau Public, GitHub  
- **Visualization**: Tableau Interactive Dashboard

## 📂 Project Structure

```
CP372-PR-PB-DataAnalytics-BusinessIntelligence/
├── 📊 EDA & In-Depth Analysis & Visualization (tableau)/
│    ├── 📄 EDA & In-Depth Analysis & Visualization (tableau).twbx
│    ├── 🖼️ EDA (Screenshot)/
│    │    ├── Sheet 1 - Bangkok Listing Density.png
│    │    ├── Sheet 2 - Listing Ratings by Category.png
│    │    ├── Sheet 3 - Avg Price per Property Type.png
│    │    ├── Sheet 4 - Premium Neighbourhoods (Top 5 by Avg Price).png
│    │    ├── Sheet 5 - Top 10 Most Listed Areas.png
│    │    ├── Sheet 6 - Average Price by Room Type.png
│    │    ├── Sheet 7 - Avg Monthly Price by Bucket (each year).png
│    │    ├── Sheet 8 - Review Scores by Category (2020).png
│    │    ├── Sheet 8 - Review Scores by Category (2024).png
│    │    ├── Sheet 9 - Minimum Nights Stay.png
│    │    ├── Sheet 10 - Entire Homes by Neighbourhood.png
│    │    └── Sheet 11 - Price vs. Review Activity.png
│    │    └── Sheet 12 - Listings Density.png
│    ├── 🧠 In-Depth Analysis (Screenshot)/
│    │    ├── Question1.png
│    │    ├── Question2.png
│    │    ├── Question3.png
│    │    ├── Question4.png
│    │    └── Question5.png
│    └── 📊 Dashboard (Screenshot)/
│         ├── (Overview) Airbnb Analysis Dashboard.png
│         ├── (Price Analysis) Airbnb Analysis Dashboard.png
│         └── (Community Impact) Airbnb’s Effect on Housing & Demand.png
│
├── 🧹 Data Preparation (colab)/
│    └── 📓 data preparation.ipynb
│
├── 📂 Data/
│    ├── 📁 cleaned data/
│    │     └── bngkok_airbnb_cleaned_v5.csv
│    └── 📁 raw data/
│          └── listings.csv
│
├── 🧾 Project Canvas/
│    ├── ProjectCanvas_CP371_Pinthucha421_Parinya119.png
│    └── ProjectCanvas_CP371_Pinthucha421_Parinya119.pdf
│
└── 📘 README.md
```

## 📝 Project Canvas

| Project Canvas |             
|------------------------------------------------|
| ![](Project%20Canvas/ProjectCanvas_CP371_Pinthucha421_Parinya119.png)  |

# 🧭 Exploratory Data Analysis (EDA)

In this section, we explore key patterns in Bangkok's Airbnb market using data visualizations and interactive dashboards. Each analysis (12 sheets) is designed to support business insights and strategic decisions.

---
 ### 🗺️ Sheet 1 – Bangkok Listing Density 

🔗 [Link to Sheet 1 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet1-BangkokListingDensity?publish=yes)
 
| Sheet 1 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%201%20-%20Bangkok%20Listing%20Density.png)  |

**Map** แสดงการกระจายของที่พัก Airbnb ทั่วกรุงเทพฯ โดยใช้พิกัดจริงจากข้อมูล  
- **Dot color** แทนประเภทห้องพัก:  
      🟦 Entire Home **·** 🟧 Hotel Room **·** 🟥 Private Room **·** 🟩Shared Room  
- สัญลักษณ์ ⭐ แสดงที่พักในเขตใจกลางเมือง เช่น วัฒนา, คลองเตย, ห้วยขวาง, ราชเทวี, สาทร  
- ช่วยให้เห็นแนวโน้มว่าที่พักประเภทไหนกระจุกตัวอยู่ในเขตใดของเมือง

**💡 Strategic Recommendations:**

- **ปรับกลยุทธ์การตั้งราคาตามพื้นที่และประเภทห้องพัก**  
  ในเขตที่มีการแข่งขันสูง (เช่น วัฒนา) ควรใช้กลยุทธ์ราคายืดหยุ่น หรือเพิ่มจุดขายพิเศษ เช่น สิ่งอำนวยความสะดวก หรือบริการเสริม

- **ส่งเสริมการกระจายตัวของที่พักไปยังพื้นที่รอบนอก**  
  สนับสนุนเจ้าของที่พักในย่านใหม่ๆ ด้วยการทำแคมเปญส่งเสริม เช่น โปรโมตสถานที่ท่องเที่ยวรอบนอก หรือให้ค่าคอมมิชชั่นพิเศษ

---

### ⭐ Sheet 2 – Listing Ratings by Category

🔗 [Link to Sheet 2 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet2-ListingRatingsbyCategory?publish=yes)

| Sheet 2 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%202%20-%20Listing%20Ratings%20by%20Category.png)  |


**Bar Chart** แสดงจำนวนที่พัก Airbnb ในแต่ละช่วงคะแนนรีวิว  

- แบ่งเป็น 5 กลุ่ม:  
  🟢 4.5+ **·** 🔵 4.0–4.49 **·** 🟡 3.5–3.99 **·** 🟠 3.0–3.49 **·** ⚪ No Rating
- ข้อมูลถูกกรองตามแต่ละเขตของกรุงเทพฯ (เลือกเปิด/ปิดได้ทางด้านขวา)  
- ช่วยให้เห็นภาพรวมคุณภาพของที่พักในแต่ละพื้นที่จากมุมมองของผู้เข้าพัก  

**Insight:**  
> มากกว่า 70% ของที่พักทั้งหมดได้คะแนนรีวิว 4.5+ สะท้อนว่าผู้เข้าพักส่วนใหญ่พึงพอใจ  
> แต่ยังมีจำนวนที่พักไม่มีคะแนนรีวิวอยู่มากกว่า 5,000 รายการ ซึ่งอาจเป็นที่พักใหม่หรือยังไม่ค่อยมีผู้เข้าพัก

**💡 Strategic Recommendations:**

- **กระตุ้นให้ผู้เข้าพักเขียนรีวิว**  
  ใช้ระบบแจ้งเตือน หรือเสนอส่วนลดในครั้งถัดไปเพื่อแลกกับการรีวิว  
  ยิ่งมีรีวิวเยอะ ยิ่งเพิ่มโอกาสถูกจองในอนาคต

- **ช่วยที่พักใหม่ให้ได้รีวิวแรกเร็วขึ้น**  
  สร้างแคมเปญ “ที่พักน้องใหม่” พร้อมราคาพิเศษหรือโบนัสสำหรับผู้เข้าพักที่รีวิว  
  ช่วยให้ที่พักใหม่มีโอกาสเข้าสู่ตลาดได้เร็วและแข่งขันได้มากขึ้น

---

### 📊 Sheet 3 - Avg Price per Property Type

🔗 [Link to Sheet 3 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet3-AvgPriceperPropertyType?publish=yes)

| Sheet 3 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%203%20-%20Avg%20Price%20per%20Property%20Type.png) |

**Bar Chart** แสดงราคาเฉลี่ยต่อคนของที่พักแต่ละประเภทในกรุงเทพฯ โดยจำแนกตาม Property Type (ประเภทของที่พัก)

**Insight:**
> - ประเภท Entire Place (เช่น Villa, Cottage, Bungalow) มีราคาสูงกว่าค่าเฉลี่ย (฿1,000+) อย่างชัดเจน เหมาะกับกลุ่มครอบครัวหรือผู้ที่ต้องการความเป็นส่วนตัว
> - Entire Cottage มีราคาสูงสุด (~฿5,799) อาจเกิดจากที่พักเฉพาะทางหรือข้อมูลจำนวนน้อย
> - Serviced Apartment และ Villa มักถูกใช้โดยกลุ่มนักท่องเที่ยวที่พักระยะกลางถึงยาวหรือผู้ต้องการสิ่งอำนวยความสะดวกครบครัน
> - Private Room และ Shared Room มีราคาต่ำกว่าเฉลี่ย (~฿200–900) ตอบโจทย์นักเดินทางคนเดียวหรืองบน้อย
> - มีบางประเภทเฉพาะ เช่น Tiny Home, Hut, Shipping Container ที่สะท้อนความหลากหลายของตลาด Airbnb

**💡 Strategic Recommendations:**
- เจ้าของ Entire Place ควรเน้นกลุ่มเป้าหมายที่ต้องการความเป็นส่วนตัวและพร้อมจ่าย เช่น นักท่องเที่ยวกลุ่มเพื่อนหรือครอบครัว
- ที่พักราคาต่ำกว่าเฉลี่ย ควรใช้กลยุทธ์เน้นความคุ้มค่า ความสะอาด และประสบการณ์ท้องถิ่น เพื่อดึงดูดนักท่องเที่ยวแบบประหยัด
- การระบุจุดขายเฉพาะของที่พัก (เช่น Tiny Home ที่แปลกใหม่) สามารถใช้ชูจุดเด่นในตลาดเฉพาะกลุ่มได้

---

### 📊 Sheet 4 - Premium Neighbourhoods (Top 5 by Avg Price)

🔗 [Link to Sheet 4 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet4-PremiumNeighbourhoodsTop5byAvgPrice?publish=yes)

| Sheet 4 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |


**Bar Chart** แสดงว่า ย่านไหนในกรุงเทพฯ ที่มีราคาที่พักเฉลี่ยต่อคนสูงที่สุดบน Airbnb  
ซึ่งสะท้อนถึงทำเลระดับพรีเมียมที่นักท่องเที่ยวอาจต้องจ่ายแพงกว่าปกติ

📌 ใช้ค่า *"Avg. Price Per Person"* = price / accommodates  
เพื่อให้การเปรียบเทียบราคาที่พักยุติธรรมและแม่นยำ  
(เช่น บ้านพัก 4 คน 4,000 บาท → 1,000 บาท/คน)

📍 Top 5 ย่านที่ราคาสูงสุด:
- **Dusit** – เฉลี่ย 1,753.8 บาท/คน/คืน  
- **Sathon** – เฉลี่ย 1,515.6 บาท/คน/คืน  
- **Pathum Wan** – เฉลี่ย 1,490.3 บาท/คน/คืน  
- **Vadhana** – เฉลี่ย 1,385.9 บาท/คน/คืน  
- **Yan Nawa** – เฉลี่ย 1,202.4 บาท/คน/คืน  

**Insight:**
> ย่านเหล่านี้มักเป็นเขตเศรษฐกิจ มีห้าง โรงแรม สำนักงาน และระบบขนส่งดีเยี่ยม  
> ราคาสูงอาจสะท้อนถึง:
> - ความต้องการจากนักท่องเที่ยวต่างชาติที่มีกำลังซื้อ  
> - ที่พักหรู เช่น Villa, Serviced Apartment, Luxury Condos  

**💡 Strategic Recommendations:**
- เจ้าของที่พักสามารถใช้ข้อมูลนี้เพื่อวางกลยุทธ์ตั้งราคาให้เหมาะสมกับทำเล
- นักลงทุนสามารถใช้ Insight นี้ในการเลือกทำเลสำหรับลงทุนในระยะยาว
- นักท่องเที่ยวสามารถใช้เพื่อวางแผนงบประมาณล่วงหน้า หรือเลือกย่านที่คุ้มค่ากว่า

---

### 📊 Sheet 5 - Top 10 Most Listed Neighbourhoods

🔗 [Link to Sheet 5 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet5-Top10MostListedAreas?publish=yes)

| Sheet 5 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%205%20-%20Top%2010%20Most%20Listed%20Areas.png) |

**Tree Map** แสดง 10 อันดับย่านในกรุงเทพฯ ที่มีจำนวนประกาศที่พัก (listings) บน Airbnb มากที่สุด

- พื้นที่ขนาดใหญ่และสีเข้ม = ย่านที่มีจำนวนที่พักมาก  
- ใช้ `CNT(Neighbourhood)` เป็น Measure  
- ใช้ `Neighbourhood Cleansed` เป็น Dimension

📍 Top 3 ย่านที่มีจำนวน listings สูง:
- **Vadhana** (ทองหล่อ เอกมัย) – มากกว่า 2,000 รายการ  
- **Khlong Toei** (อโศก พระราม 4) – รองลงมา  
- **Huai Khwang** – แม้ไม่ใช่กลางเมืองแต่ listings สูง แสดงถึงความนิยมและการเติบโต

**Insight:**
> ย่านอย่าง **Phra Nakhon**, **Suanluang**, และ **Chatuchak** ก็ติดอันดับ  
> สะท้อนการขยายตัวของที่พักไปยังพื้นที่รอบนอกนอกเขต CBD

**💡 Strategic Recommendations:**
- ผู้ประกอบการควรพิจารณาย่านที่มี demand สูงแต่ supply ยังไม่อิ่มตัว
- ในย่านที่มีการแข่งขันสูง ควรเน้นคุณภาพบริการ รีวิวดี และการตั้งราคาที่แข่งขันได้
- นักท่องเที่ยวสามารถเลือกย่านที่มีตัวเลือกมาก เพื่อเพิ่มโอกาสเจอที่พักที่ตรงใจ

---

### 🧾 Sheet 6: Average Price by Room Type

🔗 [Link to Sheet 6 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet6-AveragePricebyRoomType?publish=yes)

| Sheet 6 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |

**Horizontal Bar Chart** นี้แสดงราคาเฉลี่ยของที่พักแต่ละประเภท (Room Type) ในแต่ละย่าน (Neighbourhood) ของกรุงเทพฯ

**4 ประเภทห้องพัก:**
- 🏠 **Entire home/apt** — ประเภทนี้มีราคาเฉลี่ยสูงสุด  
  - เช่น **Lat Phrao** เฉลี่ย **฿6,083**, **Khlong Sam Wa** เฉลี่ย **฿5,671**  
  - เหมาะกับนักลงทุนที่ต้องการผลตอบแทนสูงในทำเลดี

- 🧍‍♂️ **Private room** — ตัวเลือกยอดนิยม ราคาย่อมเยา  
  - เช่น **Bang Rak** เฉลี่ย **฿2,871**, **Vadhana** เฉลี่ย **฿3,925**  
  - เหมาะกับนักเดินทางเดี่ยวหรือคู่รัก

- 🛏️ **Shared room** — ราคาต่ำสุดในทุกย่าน  
  - เช่น **Thung Khru** เฉลี่ยเพียง **฿480**, **Sathon** เฉลี่ย **฿500**  
  - เหมาะกับแบ็คแพ็คเกอร์หรือผู้มีงบจำกัด

- 🏨 **Hotel room** — ราคาปานกลาง มีความสม่ำเสมอมากกว่าห้องอื่น ๆ  
  - เช่น **Khlong Toei** เฉลี่ย **฿3,657**, **Pra Wet** เฉลี่ย **฿1,064**
  
**💡 Strategic Recommendations:**
- วางแผนเลือกประเภทห้องให้เหมาะกับแต่ละย่าน
- นักลงทุนเลือกลงทุนแบบ Entire Home ในย่านราคาสูง หรือ Private Room ในย่านยอดนิยม
- นักท่องเที่ยวสามารถใช้วางแผนงบประมาณได้

---

### 📈 Sheet 7: Average Monthly Price by Bucket

🔗 [Link to Sheet 7 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet7-AvgMonthlyPricebyBucketeachyear?publish=yes)

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

**Line Chart** แสดงแนวโน้มราคาเฉลี่ยรายเดือน โดยจำแนกตามระดับราคาที่พัก (Price Bucket) ตั้งแต่กลุ่ม Budget ไปจนถึง Luxury ซึ่งสะท้อนถึงพฤติกรรมการตั้งราคาตามฤดูกาลและกลุ่มเป้าหมาย

**ระดับราคา:**
- 🔴 **Luxury** — ราคาสูงสุดในตลาด  
  - สูงถึง **~฿28,000** ในช่วงเดือน **มีนาคม**  
  - แสดงถึงความอ่อนไหวต่อฤดูกาลอย่างชัดเจน

- 🔵 **Premium** — คงที่ประมาณ **฿4,000** ตลอดปี  
  - อาจได้รับผลกระทบจากฤดูกาลบ้างแต่ไม่เด่นชัด

- 🟢 **Standard** — อยู่ในช่วง **฿1,700–฿1,880**  
  - มีความคงที่ดี เหมาะกับตลาดกลุ่มกลาง

- 🔷 **Affordable** — ต่ำกว่า **฿800**  
  - ราคาไม่ค่อยผันผวน มีความสม่ำเสมอสูง

- 🟠 **Budget** — ต่ำสุด ราว **฿750–฿780**  
  - กลุ่มนี้ไม่ค่อยขึ้นลงตามฤดูกาล เหมาะกับลูกค้างบน้อย

**💡 Strategic Recommendations:**
- **Luxury**: ปรับราคาขึ้นในช่วง High Season (เช่น มีนาคม) เพื่อเพิ่มรายได้
- **Budget & Affordable**: รักษาระดับราคาคงที่ สร้างจุดขายเรื่องราคาถูก
- **Targeting**: แยกกลุ่มลูกค้าอย่างชัดเจน เช่น นักท่องเที่ยวระดับสูง vs. แบ็คแพ็คเกอร์
- **Promotions**: เสนอโปรโมชันในช่วงราคาตก (Low Season) เพื่อกระตุ้นยอดจองให้มากขึ้น

---

### 🌟 Sheet 8: Review Scores by Category (เปรียบเทียบปี 2020 และ 2024)

🔗 [Link to Sheet 8 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet8-ReviewScoresbyCategory?publish=yes)

<table>
  <tr>
    <td align="center" style="border:1px solid #ccc; padding:10px;">
      <strong>📅 ปี 2020</strong><br>
      <img src="EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%208%20-%20Review%20Scores%20by%20Category%20(2020).png" width="100%" alt="Review Scores 2020">
    </td>
    <td align="center" style="border:1px solid #ccc; padding:10px;">
      <strong>📅 ปี 2024</strong><br>
      <img src="EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%208%20-%20Review%20Scores%20by%20Category%20(2024).png" width="100%" alt="Review Scores 2024">
    </td>
  </tr>
</table>

**Box + Jitter Plot** เพื่อเปรียบเทียบคะแนนรีวิวจากผู้เข้าพักระหว่างปี **2020** และ **2024** ครอบคลุม 4 หมวดหลัก:

- 🕐 **Check-in**  
- 🧼 **Cleanliness**  
- 🗣️ **Communication**  
- 📍 **Location**

**Insight:**
> - ✅ **ปี 2024** มีคะแนนรีวิวโดยรวมที่สูงขึ้นในทุกหมวด โดยเฉพาะ **Communication** และ **Cleanliness** ที่คะแนนกระจุกตัวอยู่ในช่วง **4.6–4.8** แสดงถึงความพึงพอใจและความเสถียรในการให้บริการ  
> - ⚠️ **ปี 2020** มีคะแนนกระจายตัวมากกว่า และพบ **outliers** หลายจุด โดยเฉพาะในหมวด **Check-in** และ **Location** ที่มีบางรีวิวให้คะแนนต่ำถึง **3.5–3.8**  
> - 🆙 แสดงให้เห็นถึง **แนวโน้มการพัฒนา** ด้านคุณภาพการบริการของที่พัก Airbnb ในกรุงเทพฯ เมื่อเทียบระหว่างสองปี

### 💡 Strategic Recommendations

- รักษามาตรฐานบริการในหมวด **Communication** และ **Cleanliness** ที่ทำได้ดีในปี 2024
- วิเคราะห์ปัญหาที่เกิดขึ้นในปี 2020 เช่น การ Check-in ที่ล่าช้าหรือข้อมูล Location ที่ไม่ชัดเจน และควรที่จะปรับปรุงอย่างต่อเนื่อง  
- นำ **คะแนนรีวิวที่ดี** มาใช้เป็นจุดเด่นของ **กลยุทธ์ทางการตลาด** เพื่อดึงดูดลูกค้าใหม่  
- สำหรับพื้นที่ที่ยังได้คะแนน Location ต่ำ อาจต้องพิจารณาปรับ **ราคาให้สอดคล้องกับความสะดวกในการเดินทาง**
---

### 🛏️ Sheet 9: Minimum Nights Stay

🔗 [Link to Sheet 9 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet9-MinimumNightsStay?publish=yes)

| Sheet 9 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%209%20-%20Minimum%20Nights%20Stay.png) |

**Bar Chart** แสดงจำนวนที่พักตามจำนวนคืนขั้นต่ำที่ต้องจอง

**สีของแท่ง:**
- 🟥 Short-Term (<28 คืน)
- 🟫 Long-Term (≥28 คืน)

**Insight:**
> - มากกว่า 2,900 ที่พักตั้งขั้นต่ำ = 1 คืน
> - 28 คืนขึ้นไป เริ่มมีบ้าง เช่น 410 รายการ (หลีกเลี่ยงกฎหมาย STR)

**💡 Strategic Recommendations:**
- ตั้งขั้นต่ำ 1–3 คืนเพื่อเพิ่มยอดจอง
- พิจารณาเปลี่ยนโมเดลเป็นรายเดือนในบางย่าน
- จัดโปรโมชันตามระยะเวลาพัก
- วิเคราะห์แนวโน้มตลาด (short-term → long-term)

---

### 📊 Sheet 10: Entire Homes by Neighbourhood

🔗 [Link to Sheet 10 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet10-EntireHomesbyNeighbourhood?publish=yes)

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png) |

**Bar Chart** แสดงจำนวนรายการ `Entire home/apt` ในแต่ละย่านของกรุงเทพฯ  
เพื่อดูว่าย่านไหนที่เจ้าของปล่อยเช่าทั้งหลังมากที่สุด

#### 🔍 วิธีการวิเคราะห์
- **กรอง Room Type**: เฉพาะ `Entire home/apt`
- **วัดผล**: Distinct Count ของที่พักในแต่ละย่าน

#### 🏆 ย่านที่มี Entire Homes สูงสุด 5 อันดับแรก
| อันดับ | ย่าน | จำนวนรายการ |
|--------|------|--------------|
| 1️⃣ | Watthana | 11,432 |
| 2️⃣ | Khlong Toei | 9,280 |
| 3️⃣ | Huai Khwang | 7,660 |
| 4️⃣ | Ratchathewi | 3,396 |
| 5️⃣ | Sathon | 2,792 |

**Insight:**
> - บ่งชี้ว่าย่านเหล่านี้เป็นศูนย์กลางธุรกิจและไลฟ์สไตล์
> - มีแนวโน้มที่เจ้าของจะลงทุนปล่อยเช่าระยะสั้น
> - เหมาะกับกลุ่มนักท่องเที่ยวหรือครอบครัวที่ต้องการความเป็นส่วนตัว

**💡 Strategic Recommendations:**
- วิเคราะห์ความอิ่มตัวของตลาดแต่ละย่าน
- นักวางแผนเมืองหรือหน่วยงานกำกับดูแลที่เกี่ยวข้องสามารถประเมินผลกระทบต่อชุมชน
- นักท่องเที่ยวสามารถใช้เลือกทำเลที่เหมาะกับไลฟ์สไตล์ของตนเองได้

---

### 📊 Sheet 11: Price vs. Review Activity

🔗 [Link to Sheet 11 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet11-Pricevs_ReviewActivity?publish=yes)

| Sheet 11 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2011%20-%20Price%20vs.%20Review%20Activity.png) |

**Scatter Plot** แสดงความสัมพันธ์ระหว่าง **ราคาต่อคน** กับ **จำนวนรีวิวต่อเดือน**  
เพื่อวิเคราะห์ว่า "ที่พักแบบไหนราคาเท่าไรถึงได้รับความนิยม?"

#### 🎯 ค่าที่แสดงในแผนที่
- 🎨 สีของจุด (ตาม Room Type)
  - 🔵 Entire home/apt
  - 🟠 Hotel room
  - 🔴 Private room
  - 🟢 Shared room
- **ขนาดจุด**: จำนวนรีวิวรวม (Total Reviews)
- **Trend Line**: เส้นเทรนด์ของแต่ละ Room Type

#### 🔍 Insight โดย Room Type
- 🔴 **Private Room**:
  - ได้รีวิวต่อเดือนเยอะ โดยเฉพาะราคาต่ำ (< 500 บาท)
  - ยิ่งราคาถูก → ยิ่งมีรีวิว
  - เหมาะกับนักเดินทางงบจำกัด

- 🟠 **Hotel Room**:
  - ราคาสูงแต่รีวิวน้อย
  - เทรนด์ลดลงแรง → ราคาแพงเกินไปอาจไม่คุ้มค่า

- 🔵 **Entire Home/Apt**:
  - ราคาคงที่ (~1,000 บาท/คน)
  - ความนิยมไม่ขึ้นกับจำนวนรีวิวมากนัก

- 🟢 **Shared Room**:
  - จำนวนรายการน้อย
  - ราคาถูกที่สุด และได้รีวิวมากเมื่อราคาต่ำ

**💡 Strategic Recommendations:**
- ช่วยกำหนดกลยุทธ์การตั้งราคา:
  - `Private Room`: ควรตั้งราคาประหยัด
  - `Hotel Room`: ควรเพิ่มมูลค่าบริการให้สมราคา
  - `Entire Home`: เน้นความเป็นส่วนตัว ไม่ต้องลดราคา
- ใช้รีวิว/เดือน เป็นตัวแทนของ **Demand**

---

### 🗺️ Sheet 12: Listing Density Heatmap

🔗 [Link to Sheet 12 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/Sheet12-ListingsDensity?publish=yes)

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2012%20-%20Listings%20Density.png) |

**Map** แสดงความหนาแน่นของที่พัก Airbnb  
เพื่อดูว่าพื้นที่ใดมีความถี่ของ listing มาก-น้อย

#### 🎯 ค่าที่แสดงในแผนที่
- **สีของจุด** = ระดับความหนาแน่น:
  - 🟥 Very High
  - 🟧 High
  - 🟩 Low
- **ขนาดจุด** = จำนวน Listing เฉลี่ย (AVG(# Listings))

#### 🔴 โซน Very High Density
- ย่านยอดนิยม: ปทุมวัน, ทองหล่อ, สยาม, อโศก, สุขุมวิท, บางรัก  
- เหตุผล:
  - ใกล้รถไฟฟ้า
  - มีห้าง/ที่เที่ยวเยอะ
  - สะดวกกับนักท่องเที่ยวที่ไม่ใช้รถ

#### 🟧 โซน High Density
- ย่านรอบศูนย์กลาง เช่น ดินแดง, พญาไท, ห้วยขวาง, บางนา → มีโอกาสเติบโตสูง

#### 🟩 โซน Low Density
- รอบนอกเมือง เช่น นนทบุรี, สมุทรปราการ → เหมาะกับกลุ่มที่เน้นราคาถูก หรือทำเลเฉพาะ

**💡 Strategic Recommendations:**
- วิเคราะห์ทำเลที่ยังไม่อิ่มตัว ขยายที่พัก/สาขาใหม่
- วางกลยุทธ์ราคา เมื่อเกิดคู่แข่งมากต้องแข่งขันด้านคุณภาพ/ราคา
- ใช้ประกอบรายงานเพื่อเสนอต่อผู้บริหาร/นักลงทุน

---

#  🧠 Airbnb Bangkok Insights – In-Depth Analysis

การวิเคราะห์เชิงลึกนี้มุ่งเน้นไปที่การตอบคำถามสำคัญจากข้อมูล **Airbnb Listings ในกรุงเทพฯ** โดยใช้เทคนิคเชิงสถิติและการพยากรณ์เบื้องต้น เช่น **Correlation Analysis** และ **Linear Regression** เพื่อให้ได้ข้อเสนอเชิงกลยุทธ์ในการวิเคราะห์ตลาดที่พักระยะสั้น โดยมีทั้งหมด 5 คำถาม ในการวิเคราะห์เชิงลึก

## 📌 1. ย่านใดในกรุงเทพฯ ที่มีศักยภาพในการปล่อยเช่าระยะสั้นสูงที่สุด?

เพื่อประเมินศักยภาพของแต่ละย่านในการปล่อยเช่าระยะสั้น ได้มีการสร้างตัวแปรใหม่ชื่อว่า `Total_Score` โดยคำนวณจากสูตร:

```python
Total_Score = (review_scores_rating * 2) + (number_of_reviews * 0.1) - (price / 100)
```

### 🧮 เหตุผลที่เลือกใช้แต่ละตัวแปร:

| ตัวแปร                  | ความหมาย                           | เหตุผลที่เลือกใช้                                                                          | น้ำหนักที่ใช้ในสูตร                    |
|------------------------|------------------------------------|--------------------------------------------------------------------------------------------|-----------------------------------------|
| `review_scores_rating` | คะแนนรีวิวจากผู้เข้าพัก (0–100)         | สะท้อนคุณภาพที่พัก — ยิ่งคะแนนสูง แสดงถึงความพึงพอใจของผู้เข้าพัก                         | ×2 (ให้ความสำคัญสูง)                    |
| `number_of_reviews`    | จำนวนรีวิวทั้งหมด                       | แสดงความนิยมและความต้องการของผู้เข้าพัก                                                 | ×0.1 (ระดับรอง เพื่อป้องกัน bias จากย่านใหญ่) |
| `price`                | ราคาเฉลี่ยต่อคืน (บาท)                | ใช้เป็นตัวถ่วง เพราะราคาที่สูงเกินไปจะลดความน่าดึงดูดในการเข้าพัก                         | ÷100 (ลด scale ของราคา)                 |

### 📊 ผลลัพธ์:
จาก Bar Chart พบว่าย่านที่มีศักยภาพสูงสุด ได้แก่:

- Vadhana  
- Khlong Toei  
- Huai Khwang  
- Ratchathewi  
- และอื่นๆ ตามลำดับ

🔗 [Link to Question 1 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/1_?publish=yes)

| Question 1 ย่านใดในกรุงเทพฯ ที่มีศักยภาพในการปล่อยเช่าระยะสั้นสูงที่สุด? |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/In-Depth%20Analysis%20(Screenshot)/Question1.png) |

---

## 📌 2: ปัจจัยใดมีอิทธิพลต่อราคาที่พักต่อคืนมากที่สุด?

ใช้ Correlation Analysis และการเปรียบเทียบความสัมพันธ์เชิงเส้นระหว่าง `price` กับตัวแปรอื่นๆ:

| ตัวแปร                   | ความหมาย                  | ความเป็นไปได้ที่มีผลต่อราคา                   |
|------------------------|---------------------------|-----------------------------------------------|
| `accommodates`         | จำนวนคนที่รองรับได้         | ขนาดห้องพักมีแนวโน้มส่งผลให้ราคาสูงขึ้น       |
| `bedrooms`             | จำนวนห้องนอน              | แสดงถึงความกว้างขวางของที่พัก                |
| `room_type`            | ประเภทห้องพัก             | Entire home/apt มักมีราคาสูงกว่า              |
| `number_of_reviews`    | จำนวนรีวิว                | ความนิยมอาจส่งผลต่อราคาทางอ้อม                |
| `review_scores_rating` | คะแนนรีวิว                 | ส่งผลต่อมูลค่ารับรู้ (Perceived Value)        |
| `is_central`           | อยู่ใจกลางเมืองหรือไม่        | ทำเลที่ดีอาจส่งผลให้ราคาสูงขึ้น                |

### 📈 กราฟและการเปรียบเทียบ:

| Chart                                | คำอธิบาย                                      |
|-------------------------------------|-----------------------------------------------|
|**Lines Chart:** Price vs Accommodates      | ความสัมพันธ์ระหว่างขนาดห้องพักกับราคา        |
|**Lines Chart:** Price vs Bedrooms         | เปรียบเทียบราคากับจำนวนห้องนอน             |
|**Lines Chart:** Price vs Review Score      | คุณภาพกับราคา                           |
|**Bar Chart:** Price vs Room Type         | เปรียบเทียบราคาในแต่ละประเภทห้อง             |
|**Bar Chart:** Avg Price by Is Central  | ทำเลใจกลางเมืองส่งผลต่อราคาหรือไม่            |

### ✅ สรุป:
- `Accommodates` และ `Bedrooms` มีความสัมพันธ์เชิงบวกกับราคา (R² สูง)
- `Entire home/apt` มีราคาสูงกว่าประเภทอื่นชัดเจน
- ที่พักในพื้นที่ใจกลางเมือง (`is_central = 1`) มีราคาเฉลี่ยสูงกว่า

🔗 [Link to Question 2 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/2_?publish=yes)

| Question 2 ปัจจัยใดมีอิทธิพลต่อราคาที่พักต่อคืนมากที่สุด? |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/In-Depth%20Analysis%20(Screenshot)/Question2.png) |

---

## 📌 3: ราคาที่พักต่อคนสัมพันธ์กับจำนวนรีวิวต่อเดือนหรือไม่?

ต้องการทราบว่าที่พักที่มีราคาต่อคนสูง จะส่งผลต่อจำนวนรีวิวต่อเดือนหรือไม่

### 📌 ตัวแปรที่ใช้:
- `Reviews Per Month`: จำนวนรีวิวต่อเดือน
- `price_per_person`: ราคาต่อคน (คำนวณจาก `price ÷ accommodates`)

### 📉 การวิเคราะห์:
ใช้ Scatter Plot แสดงความสัมพันธ์ระหว่าง ราคาต่อคน กับ จำนวนรีวิวต่อเดือน

| ประเภทห้องพัก                        | สมการ                                      | ค่า P-value                        | นัยสำคัญทางสถิติ                                      |
|-------------------------------------|-----------------------------------------------|-------------------------------------|-----------------------------------------------|
| Shared room (ห้องพักรวม)              | `Price = 28.97 × Reviews/Month + 405.42`        | `0.729`          | ไม่มีนัยสำคัญ        |
| Private room (ห้องส่วนตัว)             | `Price = -48.95 × Reviews/Month + 988.14`       | `0.275`            | ไม่มีนัยสำคัญ        |
| Hotel room (ห้องพักแบบโรงแรม)         | `Price = -55.55 × Reviews/Month + 786.50`       | `< 0.0001`             | มีนัยสำคัญ        |

### 📈 สรุปผล:
- ห้องพักแบบโรงแรม (Hotel room) มีความสัมพันธ์เชิงลบอย่างมีนัยสำคัญระหว่าง “จำนวนรีวิวต่อเดือน” กับ “ราคาที่พักต่อคน” กล่าวคือ:
  - หากจำนวนรีวิวต่อเดือนเพิ่มขึ้น ราคาต่อคนมีแนวโน้มลดลง
  - สมการระบุว่าเมื่อรีวิวต่อเดือนเพิ่ม 1 ครั้ง ราคาต่อคนจะลดลงประมาณ 55.55 บาท
- สำหรับ ห้องพักรวม (Shared room) และ ห้องส่วนตัว (Private room):
  - ไม่มีนัยสำคัญทางสถิติ (P-value > 0.05)
  - จึงไม่สามารถสรุปได้ว่าจำนวนรีวิวต่อเดือนมีผลต่อราคาต่อคน

🔗 [Link to Question 3 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/3_?publish=yes)

| Question 3 ราคาที่พักต่อคนสัมพันธ์กับจำนวนรีวิวต่อเดือนหรือไม่? |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/In-Depth%20Analysis%20(Screenshot)/Question3.png) |

---

## 📌 4: ย่านที่มีการปล่อยเช่าทั้งหลังมากที่สุด มีราคาเฉลี่ยต่อคืนเป็นอย่างไรเมื่อเทียบกับย่านอื่น?

### 📍 วิธีวิเคราะห์:
- กรองเฉพาะ `room_type = Entire home/apt`
- นับจำนวน listings ในแต่ละย่าน (`neighbourhood_cleansed`)
- คำนวณราคาเฉลี่ย (`average price`)

### 📊 ตัวอย่างผลลัพธ์:

| ย่านยอดนิยม           | จำนวน Entire Home/apt | ราคาเฉลี่ยต่อคืน (บาท) |
|----------------------|------------------------|--------------------------|
| Vadhana              | 5,105                  | 2,928                    |
| Khlong Toei          | 3,447                  | 2,905                    |
| Huai Khwang          | 3,234                  | 2,907                    |
| Sathon               | 1,087                  | **5,233** (สูงที่สุด)   |

### ✅ สรุป:
- Vadhana, Khlong Toei, Huai Khwang มีจำนวน listings สูงสุด
- แต่ราคาสูงสุดกลับอยู่ที่ **Sathon** แม้มี listings จำนวนน้อย
- แสดงว่า **จำนวน listings ไม่ได้เป็นตัวชี้วัดราคาที่พัก**  แต่มีปัจจัยอื่นเช่น ทำเล, คุณภาพ, ความพรีเมียมของที่พัก มีผลมากกว่า

🔗 [Link to Question 4 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/4_?publish=yes)

| Question 4 ย่านที่มีการปล่อยเช่าทั้งหลังมากที่สุด มีราคาเฉลี่ยต่อคืนเป็นอย่างไรเมื่อเทียบกับย่านอื่น? |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/In-Depth%20Analysis%20(Screenshot)/Question4.png) |

---

## 📌 5: ย่านใดมี Entire Home/apt มากที่สุด และอาจได้รับผลกระทบจาก Short-Term Rentals (STR) สูงสุด?

### 🔎 วิธีประเมิน:
- เลือกเฉพาะ `room_type = Entire home/apt`
- จัดอันดับจำนวนรายการ (`listings`) ต่อย่าน
- พิจารณาร่วมกับตัวแปร `is_central` (แสดงว่าทำเลอยู่ใจกลางเมือง)

### 📍 ผลลัพธ์:

| ย่านยอดนิยม         | จำนวน Entire Home/apt | อยู่ใจกลางเมืองหรือไม่ (`is_central`) |
|--------------------|------------------------|-----------------------------------------|
| Vadhana            | 2,358                  | ✅                                       |
| Khlong Toei        | 1,935                  | ✅                                       |
| Huai Khwang        | 1,668                  | ✅                                       |

### ⚠️ ความเสี่ยง:
- STR จำนวนมากอาจส่งผลต่อ:
  - ราคาอสังหาริมทรัพย์ของคนท้องถิ่น
  - การเปลี่ยนแปลงโครงสร้างชุมชน
  - ความขัดแย้งกับผู้อยู่อาศัยระยะยาว

### ✅ สรุป:
- ย่าน Vadhana, Khlong Toei, และ Huai Khwang มีความเสี่ยงได้รับผลกระทบจาก STR สูง เนื่องจากมีจำนวน Entire Home/apt หนาแน่นและตั้งอยู่ใจกลางเมือง

🔗 [Link to Question 5 on Tableau Public](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/5_EntireHomeApartment?publish=yes)

| Question 5 ย่านใดมี Entire Home/apt มากที่สุด และอาจได้รับผลกระทบจาก Short-Term Rentals (STR) สูงสุด? |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/In-Depth%20Analysis%20(Screenshot)/Question5.png) |

---

# 📊 Airbnb Bangkok Insights – Insights & Recommendations

## ✅ Top 3 Actionable Insights

### 1. Entire Home Listings Clustered in Central Districts – Potential Community Disruption
ข้อมูลจาก Sheet 1 และ Sheet 10 แสดงให้เห็นว่า:
- เขต Vadhana, Khlong Toei, และ Huai Khwang มีจำนวนรายการที่พักประเภท Entire Home/Apartment มากที่สุดในกรุงเทพฯ
- บางเขตมีมากกว่า 11,000 รายการ ซึ่งสะท้อนถึง demand ที่สูงและความหนาแน่นของตลาด

จาก Sheet 12 (Heatmap) แสดงโซนสีแดงเข้มบริเวณใจกลางกรุงเทพฯ ซึ่งหมายถึงพื้นที่ที่มี listing หนาแน่นในระดับที่สูงมาก

📌 **นัยสำคัญ**:
- การกระจุกตัวของ Entire Homes ในพื้นที่ใจกลางเมือง ซึ่งเดิมเป็นพื้นที่อยู่อาศัย อาจส่งผลให้เกิด:
  - การขาดแคลนที่อยู่อาศัยสำหรับคนท้องถิ่น  
  - ราคาค่าเช่า/อสังหาริมทรัพย์พุ่งสูงขึ้น  
  - ความเสื่อมถอยของความเป็นชุมชน
- ปรากฏการณ์นี้คล้ายกับที่เกิดในหลายเมืองทั่วโลก เช่น บาร์เซโลนา หรือซานฟรานซิสโก ซึ่ง Airbnb ถูกวิจารณ์ว่าเป็นหนึ่งในปัจจัยเร่งให้เกิด **gentrification**

| Sheet 1 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%201%20-%20Bangkok%20Listing%20Density.png)  |

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png) |

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2012%20-%20Listings%20Density.png) |

---

### 2. Price per Person vs. Review Scores – No Significant Correlation

จาก In-Depth Analysis (p-value ≈ 0.305) และ Scatter Plot ใน Sheet 11:
- Scatter Plot ระหว่าง Price per Person กับ Review Scores Rating ไม่แสดงแนวโน้มที่ชัดเจน
- ค่า p-value ≈ 0.305 จากการทำ Linear Regression โดยแสดงให้เห็นว่า ไม่มีนัยสำคัญทางสถิติ

📌 **นัยสำคัญ**:
- การกำหนดราคาควรคำนึงถึง **ประสบการณ์ที่จะมอบให้ผู้เข้าพัก** มากกว่าการตั้งราคาสูงโดยไม่มี Value เพิ่ม
- ความพึงพอใจของลูกค้าขึ้นอยู่กับปัจจัยหลายด้าน เช่น ความสะอาด, การต้อนรับ, ความสะดวกในการเดินทาง, ความปลอดภัย
- การรีวิวที่ดีสามารถสร้าง **Trust และ Booking** ได้มากกว่าแค่การตั้งราคาสูง

| Sheet 11 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2011%20-%20Price%20vs.%20Review%20Activity.png) |

---

### 3. Room Type Has a Stronger Impact on Price than Location (in Some Cases)
จาก Sheet 3, 4 และ 6 พบว่า:
- ที่พักประเภท Entire Home / Villa มีราคาเฉลี่ยสูงแม้ในพื้นที่ชานเมือง (เช่น Lat Phrao ≈ 6,000 บาท)
- ประเภท Private/Shared Room มีราคาต่ำกว่า 1,000 บาท เหมาะสำหรับ budget travelers
- ย่านอย่าง Dusit, Sathon มีราคาต่อคนสูง แม้มีจำนวน listings น้อย → เป็นโอกาสสำหรับการลงทุนแบบเฉพาะกลุ่ม (niche market)

ใน Sheet 4 พบว่า:
- แม้ Dusit และ Sathon มีจำนวน listings ไม่มาก แต่ราคาต่อคนสูงมาก สะท้อนให้เห็นความหรูหราและกลุ่มลูกค้าเป้าหมายที่ต่างออกไป

📌 **นัยสำคัญ**:
- นักลงทุนไม่จำเป็นต้องลงทุนเฉพาะในย่านกลางเมืองเสมอไป
- ถ้าสร้างสินค้าหรือบริการที่ตรงกลุ่ม (เช่น Entire Villa สำหรับกลุ่มครอบครัว) ก็สามารถตั้งราคาสูงในย่านรอบนอกได้

| Sheet 3 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%203%20-%20Avg%20Price%20per%20Property%20Type.png) |

| Sheet 4 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |


| Sheet 6 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |


---

## 🧭 Stakeholder Recommendations

### 🏠 สำหรับเจ้าของที่พัก Airbnb
- **กลยุทธ์การตั้งราคาในย่านแข่งขันสูง** (เช่น Vadhana, Khlong Toei):
  - ใช้ *Flexible Pricing* ที่ปรับตามฤดูกาลหรืออัตราการเข้าพัก (อิงจาก Sheet 7)
  - ตัวอย่าง: ราคาช่วงมีนาคม – เมษายน ควรสูงขึ้นตามฤดูกาลท่องเที่ยว

- **สร้างจุดขายเสริมที่จับต้องได้**:
  - เช่น Self Check-in, ห้องครัว, สิ่งอำนวยความสะดวกที่ครบครัน, Netflix, ที่จอดรถ
  - สิ่งเหล่านี้ช่วยเพิ่ม *perceived value* แม้ราคาสูงกว่าคู่แข่ง

- **กระตุ้นการรีวิวจากลูกค้า**:
  - เสนอส่วนลดในครั้งถัดไป หากมีการรีวิวหลังการเข้าพัก
  - รีวิวที่มีจำนวนมากและดี สามารถเพิ่มความน่าเชื่อถือได้

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

---

### 🏙️ สำหรับนักวางแผนเมือง / หน่วยงานรัฐ

- **กำกับดูแล STR (Short-Term Rental)** ในย่านที่หนาแน่น:
  - พิจารณา *จำกัดจำนวน listings ต่อโฮสต์* เพื่อป้องกันการผูกขาดจากโฮสต์รายใหญ่
  - สนับสนุนโมเดล *Long-Term Leasing* ในเขตพักอาศัยแท้จริง

- **ใช้ข้อมูลจาก Sheet 5, 10 และ 12 ในการกำหนด Zoning**:
  - เช่น แบ่งพื้นที่เป็น “STR Friendly Zone” vs “Community Protection Zone”
  - บูรณาการกับข้อมูลจาก Google Mobility หรือระบบผังเมืองเพื่อการวางแผนระยะยาว

  
| Sheet 5 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%205%20-%20Top%2010%20Most%20Listed%20Areas.png) |

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png) |

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%2012%20-%20Listings%20Density.png) |

---

### 💼 สำหรับนักลงทุนด้านอสังหาริมทรัพย์
- ใช้ข้อมูลจาก Sheet 4, 6 และ 7 เพื่อ:
  - ระบุทำเลที่มี *ศักยภาพในการตั้งราคาสูง* แม้มี supply น้อย (เช่น Sathon, Dusit)
  - วิเคราะห์กลุ่มเป้าหมายเพื่อเลือก Room Type ที่ตรงความต้องการ เช่น Entire Villa สำหรับกลุ่มครอบครัว

- **Seasonal Pricing Strategy**:
  - ตั้งราคายืดหยุ่นตามฤดูกาลโดยใช้ข้อมูลจาก Sheet 7 (กลุ่ม Luxury = ราคาผันผวนสูง)
  - ขายห้อง Budget แบบคงที่ เพื่อสร้างรายได้ประจำ
  - ปรับราคาห้อง Luxury ขึ้น-ลงตาม Demand
  
| Sheet 4 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |

| Sheet 6 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/EDA%20(Screenshot)/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

---

# 🔍 Airbnb Bangkok – Visualization & Interactive Dashboard

## ✅ Dashboard 1: Overview of Listings in Bangkok

[📊 Tableau Public Dashboard 1 Link (Click Here)](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/OverviewAirbnbAnalysisDashboard?publish=yes)

| Dashboard 1 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/Dashboard%20(Screenshot)/(Overview)%20Airbnb%20Analysis%20Dashboard.png)  |

**วัตถุประสงค์:** ให้ภาพรวมของจำนวน listings, ประเภทห้องพัก, การกระจายราคา และเขตที่มีการปล่อยเช่ามากที่สุด

### 🔍 รายละเอียด:
- **แผนที่แสดงจำนวน listings ในแต่ละเขต (Neighbourhood)**
- **Bar Chart แสดงจำนวนที่พัก Airbnb ในแต่ละช่วงคะแนนรีวิว**
- **Bar Chart แสดงจำนวน listings แยกตาม Property Type**
- **Bar Chart แสดงจำนวนย่านที่มีราคาที่พักเฉลี่ยต่อคนสูงที่สุด**
- **Tree Map Top 10 เขตที่มี listings มากที่สุด**

### 📊 สรุปผลการวิเคราะห์:
- Entire Home/Apartment เป็นประเภทห้องที่มีการปล่อยเช่ามากที่สุด
- วัฒนา, คลองเตย และห้วยขวาง เป็นเขตที่มีจำนวน listings สูงที่สุด
- บางเขตเช่น Dusit และ Sathorn มีราคาเฉลี่ยสูงกว่าพื้นที่อื่น เพราะเป็นย่านที่หรูหราที่สุด
- มากกว่า 70% ของที่พักทั้งหมดได้คะแนนรีวิว 4.5+ สะท้อนว่าผู้เข้าพักส่วนใหญ่พึงพอใจ แต่ยังมีจำนวนที่พักไม่มีคะแนนรีวิวอยู่มากกว่า 5,000 รายการ ซึ่งอาจจะเป็นที่พักใหม่หรือยังไม่มีข้อมูลของที่พันนั้น

---

## ✅ Dashboard 2: Pricing Analysis

[📊 Tableau Public Dashboard 2 Link (Click Here)](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/PriceAnalysisAirbnbAnalysisDashboard?publish=yes)

| Dashboard 2 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/Dashboard%20(Screenshot)/(Price%20Analysis)%20Airbnb%20Analysis%20Dashboard.png)  |

**วัตถุประสงค์:** วิเคราะห์ปัจจัยที่ส่งผลต่อราคาห้องพัก เช่น Room Type, Host Type, Minimum Nights และทำเล

### 🔍 รายละเอียด:
- **Line Chart แสดงแนวโน้มราคาเฉลี่ยรายเดือน โดยจำแนกตามระดับราคาที่พัก (Price Bucket)**
- **Horizontal Bar Chart นี้แสดงราคาเฉลี่ยของที่พักแต่ละประเภท (Room Type)**
- **Box + Jitter Plot เพื่อเปรียบเทียบคะแนนรีวิวจากผู้เข้าพัก**

### 📊 สรุปผลการวิเคราะห์:
- Entire Home/Apartment มีราคาสูงสุดโดยเฉลี่ย
- ราคาค่าที่พักระดับ Luxury และ Premium มีแนวโน้มเพิ่มขึ้นตลอดทั้งปี
- พื้นที่ที่มีราคาสูง ได้แก่ ปทุมวัน และวัฒนา
- คะแนนรีวิวเฉลี่ยในแต่ละหมวดอยู่ในระดับ 4 ขึ้นไป โดยเฉพาะในหมวด Cleanliness และ Communication

---

## ✅ Dashboard 3: Host and Review Analysis

[📊 Tableau Public Dashboard 3 Link (Click Here)](https://public.tableau.com/app/profile/pinthucha.ruckpintuwat2585/viz/EDAIn-DepthAnalysisVisualizationtableau/CommunityImpactAirbnbsEffectonHousingDemand?publish=yes)

| Dashboard 3 |             
|------------------------------------------------|
| ![](EDA%20&%20In-Depth%20Analysis%20&%20Visualization%20(tableau)/Dashboard%20(Screenshot)/(Community%20Impact)%20Airbnb’s%20Effect%20on%20Housing%20&%20Demand.png)  |

**วัตถุประสงค์:** ศึกษาลักษณะของผู้ให้บริการ (Hosts) และพฤติกรรมการรีวิวของผู้เข้าพัก

### 🔍 รายละเอียด:
- **Bar Chart แสดงจำนวนที่พักตามจำนวนคืนขั้นต่ำที่ต้องจอง**
- **Bar Chart แสดงจำนวนรายการ Entire home/apt ในแต่ละย่านของกรุงเทพฯ**
- **Map แสดงความหนาแน่นของที่พัก Airbnb**
- **Scatter Plot แสดงความสัมพันธ์ระหว่าง ราคาต่อคน กับ จำนวนรีวิวต่อเดือน**

### 📊 สรุปผลการวิเคราะห์:
- พบว่า Host จำนวนมากมี listings มากกว่า 3 รายการ แสดงถึงแนวโน้มการให้บริการแบบเชิงพาณิชย์
- Entire home/apt เป็นประเภทห้องพักที่ได้รับความนิยมสูงที่สุด
- Listings ที่มีจำนวนรีวิวสูงมักแสดงถึงความน่าเชื่อถือ และอยู่ในพื้นที่ที่มีความต้องการสูง
- ความสัมพันธ์ระหว่างราคาและรีวิวต่อเดือนมีลักษณะแตกต่างกันในแต่ละประเภทการเข้าพัก


---
