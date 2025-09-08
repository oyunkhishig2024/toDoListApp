📝 Todo App — Learn localStorage by Building a Todo App
Энэхүү төслийн зорилго нь JavaScript ашиглан localStorage-ийн ажиллагааг сурч, хэрэглэгчийн өгөгдлийг хадгалах, шинэчлэх, устгах дадалтай болох явдал юм. FreeCodeCamp-ийн workshop-д суурилан бүтээв.

🔗 Live Demo: https://3-9-2-todo-app.vercel.app

📚 Хичээлийн зорилго
localStorage-д өгөгдөл хадгалах
DOM ашиглан UI харуулах
Форм дээр шалгалт хийх (validation)
Текстээс тусгай тэмдэгтүүдийг цэвэрлэх
🗂 Файлын бүтэц
📁 project/
├── index.html # UI бүтэц
├── styles.css # Хэрэглэгчийн интерфэйс
└── script.js # Логик болон localStorage ашиглалт

⚙️ Гол функцууд
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
