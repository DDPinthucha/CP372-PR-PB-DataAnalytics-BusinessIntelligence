# 🏙️ Airbnb Bangkok Insights <br> (วิเคราะห์ตลาดและผลกระทบของที่พักให้เช่าระยะสั้นในกรุงเทพฯ)

This project is an end-to-end data analysis project exploring the dynamics and impacts of short-term rental listings on Airbnb in Bangkok, Thailand. This project aims to deliver actionable insights through data visualizations and in-depth analysis to support stakeholders in decision-making.

## 👥 Authors

- **Pinthucha Ruckpintuwat**  
  `ID 65102010421` `pinthucha.ruckpintuwat@g.swu.ac.th`
- **Parinya Boonpama**  
  `ID 65102010119`  `parinya.boonpama@g.swu.ac.th`

## 🔗 Project Resources

- 📄 [Project Canvas](https://www.canva.com/design/DAGmXjOI3l0/ziHAPmuQZ_6Li6dkWGW9RQ/edit?utm_content=DAGmXjOI3l0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- 🧮 [Data Preparation Notebook (Colab)](https://colab.research.google.com/drive/1-02Nbqbo4TElalLMlemI1xjEYGpQB7U3?usp=sharing)
- 🔍 [Exploratory Data Analysis, EDA (Tableau)](https://your-tableau-link-here)
- 💡 [In-Depth Analysis (Tableau)](https://your-tableau-link-here)
- 📊 [Tableau Public Dashboard](https://your-tableau-link-here)
- 🎥 [Video Presentation](https://your-youtube-link-here)

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



## 📝 Project Canvas

| Project Canvas |             
|------------------------------------------------|
| ![](Project%20Canvas/ProjectCanvas_CP371_Pinthucha421_Parinya119.png)  |

## 🧭 Exploratory Data Analysis (EDA)

In this section, we explore key patterns in Bangkok's Airbnb market using data visualizations and interactive dashboards. Each analysis (12 sheets) is designed to support business insights and strategic decisions.

---
 ### 🗺️ Sheet 1 – Bangkok Listing Density 
 
| Sheet 1 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%201%20-%20Bangkok%20Listing%20Density.png)  |

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

| Sheet 2 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%202%20-%20Listing%20Ratings%20by%20Category.png)  |


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

| Sheet 3 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%203%20-%20Avg%20Price%20per%20Property%20Type.png) |

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


| Sheet 4 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |


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

| Sheet 5 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%205%20-%20Top%2010%20Most%20Listed%20Areas.png) |

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

| Sheet 6 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |

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
- นักท่องเที่ยวใช้วางแผนงบประมาณ

---

### 📈 Sheet 7: Average Monthly Price by Bucket

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

**Line Chart** แสดงแนวโน้มราคาเฉลี่ยรายเดือน โดยแบ่งตาม Price Bucket:

**ระดับราคา:**
- 🔴 Luxury: สูงสุด — สูงถึง ~28,000 บาท ในมีนาคม
- 🔵 Premium: ~4,000 บาท
- 🟢 Standard: ~1,700–1,880 บาท
- 🔷 Affordable: <800 บาท
- 🟠 Budget: ~750–780 บาท

**💡 Strategic Recommendations:**
- Luxury: ตั้งราคายืดหยุ่นตามฤดูกาล เช่น ขึ้นช่วงมีนาคม
- Budget/Affordable: รักษาระดับราคาคงที่
- วางแผนโปรโมชั่นช่วงราคาตก
- แยกกลุ่มเป้าหมายชัดเจน (Luxury vs. Budget)

---

### 🌟 Sheet 8: Review Scores by Category (เปรียบเทียบปี 2020 และ 2024)

<table>
  <tr>
    <td align="center" style="border:1px solid #ccc; padding:10px;">
      <strong>📅 ปี 2020</strong><br>
      <img src="EDA_Screenshot/Sheet%208%20-%20Review%20Scores%20by%20Category%20(2020).png" width="100%" alt="Review Scores 2020">
    </td>
    <td align="center" style="border:1px solid #ccc; padding:10px;">
      <strong>📅 ปี 2024</strong><br>
      <img src="EDA_Screenshot/Sheet%208%20-%20Review%20Scores%20by%20Category%20(2024).png" width="100%" alt="Review Scores 2024">
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
- วิเคราะห์ปัญหาที่เกิดขึ้นในปี 2020 เช่น การ Check-in ที่ล่าช้าหรือข้อมูล Location ที่ไม่ชัดเจน และปรับปรุงต่อเนื่อง  
- นำ **คะแนนรีวิวที่ดี** มาใช้เป็นจุดเด่นใน **กลยุทธ์การตลาด** เพื่อดึงดูดลูกค้าใหม่  
- สำหรับพื้นที่ที่ยังได้คะแนน Location ต่ำ อาจพิจารณาปรับ **ราคาให้สอดคล้องกับความสะดวกในการเดินทาง**
---

### 🛏️ Sheet 9: Minimum Nights Stay

| Sheet 9 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%209%20-%20Minimum%20Nights%20Stay.png) |

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

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png) |

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
- ผู้วางแผนเมืองสามารถประเมินผลกระทบต่อชุมชน
- นักท่องเที่ยวใช้เลือกทำเลที่เหมาะกับไลฟ์สไตล์

---

### 📊 Sheet 11: Price vs. Review Activity

| Sheet 11 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2011%20-%20Price%20vs.%20Review%20Activity.png) |

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
- ใช้รีวิว/เดือน เป็นตัวแทนของ **ดีมานด์**

---

### 🗺️ Sheet 12: Listing Density Heatmap

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2012%20-%20Listings%20Density.png) |

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
- วิเคราะห์ทำเลที่ยังไม่อิ่มตัว → ขยายสาขาใหม่
- วางกลยุทธ์ราคา → คู่แข่งมากต้องแข่งขันด้านคุณภาพ/ราคา
- ใช้ประกอบรายงานเพื่อเสนอต่อผู้บริหาร/นักลงทุน

---

# 📊 Airbnb Bangkok Insights – Insights & Recommendations

## ✅ Top 3 Actionable Insights

### 1. Entire Home Listings Clustered in Central Districts – Potential Community Disruption
- ย่าน **Vadhana, Khlong Toei, Huai Khwang** มีจำนวน Entire Home listings สูงมาก (มากกว่า 11,000 รายการในบางพื้นที่) *(อ้างอิงจาก Sheet 1, 10)*
- **Heatmap ใน Sheet 12** แสดงความหนาแน่นในระดับ “Very High” ในใจกลางเมือง
- แนวโน้มการเพิ่มขึ้นของ Entire Home ในย่านพักอาศัยสะท้อนถึงความเสี่ยงในการเปลี่ยนแปลงโครงสร้างชุมชน เช่น การลดลงของที่อยู่อาศัยระยะยาว

| Sheet 1 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%201%20-%20Bangkok%20Listing%20Density.png)  |

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png)  |

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2012%20-%20Listings%20Density.png) |

---

### 2. Price per Person vs. Review Scores – No Significant Correlation
- จาก **In-Depth Analysis (p-value ≈ 0.305)** และ **Scatter Plot ใน Sheet 11**
- ไม่พบความสัมพันธ์ที่ชัดเจนระหว่าง **ราคาต่อคน** กับ **คะแนนรีวิว**
- ที่พักที่มีราคาสูงไม่ได้หมายความว่าผู้เข้าพักจะพึงพอใจมากขึ้น → การปรับปรุงประสบการณ์ผู้เข้าพักสำคัญกว่าการตั้งราคาสูง

| Sheet 11 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2011%20-%20Price%20vs.%20Review%20Activity.png) |

---

### 3. Room Type Has a Stronger Impact on Price than Location (in Some Cases)
- ข้อมูลจาก **Sheet 3, 4, และ 6** ชี้ว่า:
  - ที่พักประเภท **Entire Home / Villa** มีราคาเฉลี่ยสูงแม้ในพื้นที่ชานเมือง (เช่น Lat Phrao ≈ 6,000 บาท)
  - ประเภท **Private/Shared Room** มีราคาต่ำกว่า 1,000 บาท เหมาะสำหรับ budget travelers
  - ย่านอย่าง **Dusit, Sathon** มีราคาต่อคนสูง แม้มีจำนวน listings น้อย → เป็นโอกาสสำหรับการลงทุนแบบเฉพาะกลุ่ม (niche market)

| Sheet 3 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%203%20-%20Avg%20Price%20per%20Property%20Type.png) |

| Sheet 4 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |

| Sheet 6 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |

---

## 🧭 Stakeholder Recommendations

### 🏠 สำหรับเจ้าของที่พัก Airbnb
- **ปรับกลยุทธ์ราคาในพื้นที่แข่งขันสูง** เช่น Vadhana, Khlong Toei:
  - ใช้ **Flexible Pricing** ตามฤดูกาล *(ดู Sheet 7)*
  - จัดโปรโมชั่น / ส่วนลดตามช่วงเทศกาล
- **เพิ่มจุดขายที่จับต้องได้** เช่น:
  - Self Check-in, WiFi, ห้องครัว, ความสะอาด, สิ่งอำนวยความสะดวกอื่นๆ
- **กระตุ้นการรีวิวจากลูกค้า**:
  - เสนอส่วนลดในครั้งถัดไป หากมีการรีวิวหลังการเข้าพัก

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

---

### 🏙️ สำหรับนักวางแผนเมือง / หน่วยงานรัฐ
- **ควบคุมความหนาแน่นของที่พักระยะสั้น (STR)**:
  - จำกัดจำนวน listings ต่อ host
  - ส่งเสริมการอยู่อาศัยระยะยาวในย่านที่อยู่อาศัยจริง
  - ใช้ข้อมูลจาก **Sheet 5, 10, 12** เพื่อกำหนด **โซนนิ่ง** และแนวทางกำกับดูแล
  
| Sheet 5 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%205%20-%20Top%2010%20Most%20Listed%20Areas.png) |

| Sheet 10 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2010%20-%20Entire%20Homes%20by%20Neighbourhood.png)  |

| Sheet 12 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%2012%20-%20Listings%20Density.png) |

---

### 💼 สำหรับนักลงทุนด้านอสังหาริมทรัพย์
- ใช้ข้อมูลจาก **Sheet 4, 6, 7** เพื่อ:
  - คัดเลือกทำเลราคาสูง (Top 5 Premium Neighbourhoods)
  - ลงทุนใน Entire Home ในพื้นที่ราคาสูงแต่มีคู่แข่งน้อย
  - ปรับราคาแบบ **Seasonal Strategy** แยกกลุ่ม Luxury vs Budget
  
| Sheet 4 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%204%20-%20Premium%20Neighbourhoods%20(Top%205%20by%20Avg%20Price).png) |

| Sheet 6 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%20%206%20-%20Average%20Price%20by%20Room%20Type.png) |

| Sheet 7 |             
|------------------------------------------------|
| ![](EDA_Screenshot/Sheet%207%20-%20%20Avg%20Monthly%20Price%20by%20Bucket%20(each%20year).png) |

---

📎 *ข้อมูลทั้งหมดอ้างอิงจากการวิเคราะห์ใน Tableau Dashboard และผลลัพธ์จากการวิเคราะห์เชิงลึก (In-Depth Analysis)*
