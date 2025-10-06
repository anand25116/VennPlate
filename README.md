# 🥗 HackRU 2025 — Project: VennPlate

### Challenge Partner: **Wakefern Food Corp**

---

## 🏢 About Wakefern Food Corp
Wakefern Food Corporation is the largest retailer-owned cooperative in the United States, managing popular supermarket brands like **ShopRite**, **Price Rite Marketplace**, **The Fresh Grocer**, and **Dearborn Market**.  
They focus on **sustainable retail innovation**, **data-driven consumer personalization**, and **AI-assisted shopping experiences** that improve both operational efficiency and customer satisfaction.

---

## 💡 Project Overview — *VennPlate*

**VennPlate** is an **AI-powered family meal planner** that personalizes weekly meal plans for households based on **individual dietary needs, allergies, and preferences** — all while optimizing for **shared ingredients** to reduce food waste and grocery costs.

Our goal is to bring smart, family-centered meal planning to grocery ecosystems like **Wakefern’s ShopRite**, empowering customers with tailored meal suggestions and dynamic shopping lists that integrate seamlessly with grocery inventories.

---

## 🚀 Inspiration

Meal planning for families can be stressful — especially when juggling multiple diets (vegan, keto, gluten-free, etc.).  
We wanted to build something that **bridges AI meal generation with real-world grocery data**, helping households make better food choices while keeping grocery shopping efficient and cost-effective.

---

## 🧠 What It Does

- 🧾 **Family-Aware AI Meal Planning**  
  Uses **Gemini AI (Google Generative AI)** to generate balanced, personalized 7-day meal plans.  

- 🍳 **Dietary Customization**  
  Each family member gets meal variations according to their **diet, preferences, and allergies**.

- 🛒 **Shared Grocery Optimization**  
  AI minimizes redundant ingredients — one set of groceries can serve multiple custom meals.

- ☁️ **Firebase-Integrated API**  
  Family and meal data are stored, retrieved, and updated in **Google Firestore**, making the system scalable and real-time.

- 📱 **Mobile Integration**  
  Designed to connect seamlessly with a Swift-based iOS frontend for quick API calls and user-friendly meal plan display.

---

## 🧩 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Backend API** | FastAPI (Python) |
| **AI Engine** | Gemini 2.0 Flash (Google GenAI) |
| **Database** | Google Firebase Firestore |
| **Frontend (Mobile)** | Swift (iOS app) |
| **Hosting** | Uvicorn / Local Server |
| **Environment Management** | Python `.venv` + `.env` configuration |

---

## ⚙️ How It Works

1. **Family Data Input**  
   Each family is registered in Firestore with members, dietary info, and allergies.  
2. **AI Plan Generation**  
   FastAPI endpoint `/generateMealPlan` triggers Gemini to create a JSON-based meal plan.  
3. **Meal Plan Storage**  
   Generated meal plans are saved in Firestore under each family.  
4. **Frontend Fetch**  
   The Swift app calls `/mealplan/{mealPlanId}` to render weekly meal schedules and grocery lists.

---

## 🧾 Example API Endpoints

### ▶️ Generate a Meal Plan
```bash
POST /generateMealPlan
Content-Type: application/json
{
  "familyId": "a7yM5dJr9NMKQp17VDQkFTvNfNl2"
}
```
### ▶️ Retrieve a Saved Meal Plan
```bash
GET /mealplan/{mealPlanId}
```
---
## 🔗 Relevance to Wakefern Challenge
Wakefern’s challenge centers around enhancing the food retail experience through data and AI.
VennPlate aligns directly with this mission by:

- Personalizing meal planning to drive smarter grocery choices.
- Reducing waste through shared ingredient optimization.
- Encouraging healthier diets aligned with family needs.
- Enabling digital transformation of how customers shop and plan meals — right from their homes.
  
---
## 🧑‍💻 Team VennPlate

- Anand Patel
- Santanu Agarwal
- Aparajita Sarkar
  
---
## 🏁 Future Vision

- Integrate Wakefern’s ShopRite product APIs for real-time grocery pricing.
- Add nutritional insights and budget tracking.

---
## 🥗 Why VennPlate?

“Plan smarter, shop faster, eat better — VennPlate gives you AI meal plans with ready grocery lists.”

---  
