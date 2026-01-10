📘 Express-Server — User Documentation
🧠 Project Summary

এটা একটি Node.js + Express.js based backend API server।
Express হলো Node.js এর উপর তৈরি minimalist web framework — সহজে API বা web server বানাতে ব্যবহৃত হয়।

এই সার্ভারটি বিভিন্ন HTTP endpoints বানিয়ে, browser / frontend / API client থেকে request গ্রহণ করে response দেয়।

📁 Repository Structure
express-server/
├── models/              # ডাটা (JSON / Model) সংরক্ষণের জায়গা
├── db.js                # ডাটাবেস/ডাটা সংক্রান্ত logic
├── index.js             # Express routes ও API logic
├── server.js            # Server start ও configuration
├── package.json         # Dependencies & scripts
├── README.md            # (এটা) Documentation

⚙️ Installation & Setup
🔹 Requirements

✔ Node.js ইনস্টল থাকতে হবে
✔ Terminal / CMD

🔹 Setup Steps

Clone the repository

git clone https://github.com/haisam10/express-server.git
cd express-server


Install dependencies

npm install


Run the server

node server.js


Server Status
যদি ঠিকভাবে চলে, তাহলে console এ দেখাবে যে server চলছে।
ডিফল্ট port হতে পারে 5000 (এটা তোমার কোড অনুযায়ী থাকবে)।

🌐 API Endpoints / Routes

এই API গুলো Browser বা API tool (যেমন: Postman) থেকে পরীক্ষা করা যাবে।

👇 নিচে প্রত্যেকটি route-এর বর্ণনা:

✅ GET /

➡️ রুট URL এ একটি সাধারণ response দেখাবে।
👀 Browser এ:

http://localhost:5000/

📄 GET /phone

➡️ একটি HTML page বা response প্রদর্শন করে।

http://localhost:5000/phone

👩‍🎓 Student APIs

এগুলো student-এর data provide করে:

📊 GET /students

➡️ সব student এর data return করবে।

http://localhost:5000/students

🔍 GET /students/:id

➡️ নির্দিষ্ট student ID দিয়ে student info return করবে।

http://localhost:5000/students/1

🧑‍🎓 GET /students/name/:name

➡️ student name দিয়ে search করে student info return করবে।

http://localhost:5000/students/name/shakil

📄 Simple Pages
📌 GET /about

➡️ About page বা text response।

http://localhost:5000/about

📌 GET /contact

➡️ Contact page বা text response।

http://localhost:5000/contact

🚀 Usage / Testing

✔ Browser থেকে direct hit করা যায়
✔ অথবা Postman / Insomnia এর মতো tool দিয়ে API call করা যায়

উদাহরণ:

GET http://localhost:5000/students

💡 Notes

🔹 কোডটি Express.js বেসিক routing শেখার উদ্দেশ্যে তৈরি।
🔹 এখানে কোনো পেইড বা ডাটাবেস সংযুক্ত নেই — JSON বা ফিক্সড ডাটা use হয়।
🔹 চাইলে MongoDB/MySQL যুক্ত করে REST API বানানো যায়।

🛠️ Next Steps (Optional)

✨ তুমি চাইলে এই ফিচারগুলো যোগ করতে পারো:

POST endpoint — নতুন student add করা

PUT endpoint — existing student update

DELETE endpoint — student delete

বাস্তব database integration

📚 Express.js Overview (Optional)

Express হচ্ছে Node.js-এর জন্য একটি minimalist web framework — রাউটিং, middleware, API সহজেই বানাতে সাহায্য করে।
