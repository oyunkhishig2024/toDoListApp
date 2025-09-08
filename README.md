# 📝 Todo App — Learn localStorage by Building a Todo App

Энэхүү төслийн зорилго нь JavaScript ашиглан `localStorage`-ийн ажиллагааг сурч, хэрэглэгчийн өгөгдлийг хадгалах, шинэчлэх, устгах дадалтай болох явдал юм. FreeCodeCamp-ийн workshop-д суурилан бүтээв.

🔗 **Live Demo**: [https://3-9-2-todo-app.vercel.app](https://3-9-2-todo-app.vercel.app)

---

## 📚 Хичээлийн зорилго

- `localStorage`-д өгөгдөл хадгалах
- `DOM` ашиглан UI харуулах
- Форм дээр шалгалт хийх (`validation`)
- Текстээс тусгай тэмдэгтүүдийг цэвэрлэх

---

## 🗂 Файлын бүтэц

📁 project/<br>
├── index.html # UI бүтэц<br>
├── styles.css # Хэрэглэгчийн интерфэйс<br>
└── script.js # Логик болон localStorage ашиглалт<br>

## 🧱 Neo-Brutalist UI
This update introduces a raw, vibrant, and unapologetically bold design. Inspired by brutalist architecture and digital rebellion, the interface now features:
- Thick black borders
- Vibrant color palette (hot pink, neon yellow, cyan)
- Monospace typography
- Flat, grid-based layout

Perfect for users who like their to-do lists loud and proud.


## ⚙️ Гол функцууд

```js
const removeSpecialChars = (val) => {
  return val.trim().replace(/[^A-Za-z0-9\-\s]/g, '');
};
js
Copy
Edit
const taskObj = {
  id: `${removeSpecialChars(titleInput.value).toLowerCase().split(" ").join("-")}-${Date.now()}`,
  title: removeSpecialChars(titleInput.value),
  date: dateInput.value,
  description: removeSpecialChars(descriptionInput.value),
};
