# 🚢 Titanic Survival Prediction API

Sebuah mini-proyek berbasis **FastAPI** yang dapat memprediksi kemungkinan **penumpang Titanic selamat atau tidak**, berdasarkan input karakteristik penumpang.

## 📁 Struktur File

```
├── main.py             # Endpoint API utama
├── model.pkl           # File model Machine Learning yang telah dilatih
├── scaler.pkl          # File scaler untuk normalisasi fitur input
├── requirements.txt    # Daftar dependency yang dibutuhkan
```

## 🚀 Fitur API

- Prediksi status keselamatan penumpang Titanic
- Menerima input melalui metode POST
- Hasil prediksi: `Survived` atau `Not Survived`
- Ringan, cepat, dan siap diintegrasikan ke aplikasi lain

## ⚙️ Cara Menjalankan

### 1. Clone Repositori

```bash
git clone https://github.com/namamu/titanic-fastapi.git
cd titanic-fastapi
```

### 2. Buat Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependensi

```bash
pip install -r requirements.txt
```

### 4. Jalankan API

```bash
uvicorn main:app --reload
```

### 5. Akses Swagger UI

Buka browser ke:  
👉 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

## 🧪 Contoh JSON Input

```json
{
  "Name": "John Doe",
  "Pclass": 2,
  "Sex": "male",
  "Age": 30,
  "SibSp": 1,
  "Parch": 0,
  "Fare": 13.5,
  "Embarked": "S"
}
```

## ✅ Contoh Output

```json
{
  "name": "John Doe",
  "prediction": 1,
  "result": "Survived"
}
```


> Dibuat sebagai bagian dari praktik tahap **Deployment** dalam metode **CRISP-DM**.  
> Proyek ini dapat dijadikan dasar pengembangan API prediksi sederhana lainnya.
