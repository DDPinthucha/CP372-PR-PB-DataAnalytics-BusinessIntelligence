# 🏠 Airbnb Bangkok Data Platform <br> (วิเคราะห์ ทำความเข้าใจ และวางกลยุทธ์ราคาที่พักในกรุงเทพฯ)

This project is an end-to-end data analysis project exploring the dynamics and impacts of short-term rental listings on Airbnb in Bangkok, Thailand. This project aims to deliver actionable insights through data visualizations and in-depth analysis to support stakeholders in decision-making.

## 🔗 Project Resources

- 📄 [Project Canvas](https://www.canva.com/design/DAGmXjOI3l0/ziHAPmuQZ_6Li6dkWGW9RQ/edit?utm_content=DAGmXjOI3l0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- 🧮 [Data Preparation Notebook (Colab)](https://colab.research.google.com/drive/1-02Nbqbo4TElalLMlemI1xjEYGpQB7U3?usp=sharing)
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
  
## 🧭 Exploratory Data Analysis (EDA)

In this section, we explore key patterns in Bangkok's Airbnb market using data visualizations and interactive dashboards. Each analysis is designed to support business insights and strategic decisions.

---

### 🗺️ Sheet 1 – Bangkok Listing Density

![Distribution of Airbnb Listings](EDA_Screenshot/Sheet%201%20-%20Bangkok%20Listing%20Density.png)

แผนที่แสดงการกระจายของที่พัก Airbnb ทั่วกรุงเทพฯ โดยใช้พิกัดจริงจากข้อมูล  
- **Dot color** แทนประเภทห้องพัก:  
  🟦 Entire Home · 🟧 Hotel Room · 🟥 Private Room · 🟩Shared Room  
- สัญลักษณ์ ⭐ แสดงที่พักในเขตใจกลางเมือง เช่น วัฒนา, คลองเตย, ห้วยขวาง, ราชเทวี, สาทร  
- ช่วยให้เห็นแนวโน้มว่าที่พักประเภทไหนกระจุกตัวอยู่ในเขตใดของเมือง

**💡 Strategic Recommendations:**

- **ปรับกลยุทธ์การตั้งราคาตามพื้นที่และประเภทห้องพัก**  
  ในเขตที่มีการแข่งขันสูง (เช่น วัฒนา) ควรใช้กลยุทธ์ราคายืดหยุ่น หรือเพิ่มจุดขายพิเศษ เช่น สิ่งอำนวยความสะดวก หรือบริการเสริม

- **ส่งเสริมการกระจายตัวของที่พักไปยังพื้นที่รอบนอก**  
  สนับสนุนเจ้าของที่พักในย่านใหม่ๆ ด้วยการทำแคมเปญส่งเสริม เช่น โปรโมตสถานที่ท่องเที่ยวรอบนอก หรือให้ค่าคอมมิชชั่นพิเศษ

---

### ⭐ Sheet 2 – Listing Ratings by Category

Bar Chart แสดงจำนวนที่พัก Airbnb ในแต่ละช่วงคะแนนรีวิว  

- แบ่งเป็น 5 กลุ่ม:  
  🟢 4.5+ · 🔵 4.0–4.49 · 🟡 3.5–3.99 · 🟠 3.0–3.49 · ⚪ No Rating
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

![Avg Price per Property Type](https://github.com/your-username/your-repo-name/blob/main/images/sheet3_avg_price_property_type.png)

กราฟแท่งแสดงราคาเฉลี่ยต่อคนของที่พักแต่ละประเภทในกรุงเทพฯ โดยจำแนกตาม Property Type (ประเภทของที่พัก)

- ประเภท Entire Place (เช่น Villa, Cottage, Bungalow) มีราคาสูงกว่าค่าเฉลี่ย (฿1,000+) อย่างชัดเจน เหมาะกับกลุ่มครอบครัวหรือผู้ที่ต้องการความเป็นส่วนตัว
- Entire Cottage มีราคาสูงสุด (~฿5,799) อาจเกิดจากที่พักเฉพาะทางหรือข้อมูลจำนวนน้อย
- Serviced Apartment และ Villa มักถูกใช้โดยกลุ่มนักท่องเที่ยวที่พักระยะกลางถึงยาวหรือผู้ต้องการสิ่งอำนวยความสะดวกครบครัน
- Private Room และ Shared Room มีราคาต่ำกว่าเฉลี่ย (~฿200–900) ตอบโจทย์นักเดินทางคนเดียวหรืองบน้อย
- มีบางประเภทเฉพาะ เช่น Tiny Home, Hut, Shipping Container ที่สะท้อนความหลากหลายของตลาด Airbnb

**💡 Strategic Recommendations:**
- เจ้าของ Entire Place ควรเน้นกลุ่มเป้าหมายที่ต้องการความเป็นส่วนตัวและพร้อมจ่าย เช่น นักท่องเที่ยวกลุ่มเพื่อนหรือครอบครัว
- ที่พักราคาต่ำกว่าเฉลี่ย ควรใช้กลยุทธ์เน้นความคุ้มค่า ความสะอาด และประสบการณ์ท้องถิ่น เพื่อดึงดูดนักท่องเที่ยวแบบประหยัด
- การระบุจุดขายเฉพาะของที่พัก (เช่น Tiny Home ที่แปลกใหม่) สามารถใช้ชูจุดเด่นในตลาดเฉพาะกลุ่มได้

---

### 📊 Sheet 4 - Premium Neighbourhoods (Top 5 by Avg Price)

![Premium Neighbourhoods](images/sheet4_premium_neighbourhoods.png)

กราฟแท่งแสดงว่า ย่านไหนในกรุงเทพฯ ที่มีราคาที่พักเฉลี่ยต่อคนสูงที่สุดบน Airbnb  
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

💡 ย่านเหล่านี้มักเป็นเขตเศรษฐกิจ มีห้าง โรงแรม สำนักงาน และระบบขนส่งดีเยี่ยม  
ราคาสูงอาจสะท้อนถึง:
- ความต้องการจากนักท่องเที่ยวต่างชาติที่มีกำลังซื้อ  
- ที่พักหรู เช่น Villa, Serviced Apartment, Luxury Condos  

**💡 Strategic Recommendations:**
- เจ้าของที่พักสามารถใช้ข้อมูลนี้เพื่อวางกลยุทธ์ตั้งราคาให้เหมาะสมกับทำเล
- นักลงทุนสามารถใช้ Insight นี้ในการเลือกทำเลสำหรับลงทุนในระยะยาว
- นักท่องเที่ยวสามารถใช้เพื่อวางแผนงบประมาณล่วงหน้า หรือเลือกย่านที่คุ้มค่ากว่า

---

## 📊 Sheet 5 - Top 10 Most Listed Neighbourhoods

![Top 10 Neighbourhoods](images/sheet5_top10_listed_neighbourhoods.png)

Tree Map แสดง 10 อันดับย่านในกรุงเทพฯ ที่มีจำนวนประกาศที่พัก (listings) บน Airbnb มากที่สุด

- พื้นที่ขนาดใหญ่และสีเข้ม = ย่านที่มีจำนวนที่พักมาก  
- ใช้ `CNT(Neighbourhood)` เป็น Measure  
- ใช้ `Neighbourhood Cleansed` เป็น Dimension

📍 Top 3 ย่านที่มีจำนวน listings สูง:
- **Vadhana** (ทองหล่อ เอกมัย) – มากกว่า 2,000 รายการ  
- **Khlong Toei** (อโศก พระราม 4) – รองลงมา  
- **Huai Khwang** – แม้ไม่ใช่กลางเมืองแต่ listings สูง แสดงถึงความนิยมและการเติบโต

ย่านอย่าง **Phra Nakhon**, **Suanluang**, และ **Chatuchak** ก็ติดอันดับ  
สะท้อนการขยายตัวของที่พักไปยังพื้นที่รอบนอกนอกเขต CBD

**💡 Strategic Recommendations:**
- ผู้ประกอบการควรพิจารณาย่านที่มี demand สูงแต่ supply ยังไม่อิ่มตัว
- ในย่านที่มีการแข่งขันสูง ควรเน้นคุณภาพบริการ รีวิวดี และการตั้งราคาที่แข่งขันได้
- นักท่องเที่ยวสามารถเลือกย่านที่มีตัวเลือกมาก เพื่อเพิ่มโอกาสเจอที่พักที่ตรงใจ
