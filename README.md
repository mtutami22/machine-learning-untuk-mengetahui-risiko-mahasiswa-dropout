# Mechine Learning untuk Mengetahui Risiko Mahasiswa Dropout

## Repository Outline
```
1. README.md - Penjelasan gambaran umum project
2. notebook.ipynb - Notebook yang berisi pengolahan data dengan python
3. inference.ipynb - Notebook berisi inference di mana proses prediksi mahasiswa yang datanya di input dilakukan.
4. dataset.csv - Berisi dataset yang digunakan
```

## Problem Background
```
Seperti yang diketahui, banyak mahasiswa yang merasa salah jurusan ketika sudah mengikuti pembelajaran di perguruan tinggi. Hal tersebut dapat menjadi penyebab mahasiswa kehilangan motivasi untuk mengikuti perkuliahan. Selain itu, faktor ekonomi juga dapat menyebabkan gangguan bagi kemajuan pendidikan mahasiswa. Oleh karena itu, pihak universitas ingin mengetahui mahasiswa mana yang memiliki risiko dropout sehingga dapat dibantu agar tetap bisa mengikuti perkuliahan hingga lulus.
```

## Project Output
```
Output project ini yaitu machine learning untuk melakukan prediksi status mahasiswa berupa graduate, enrolled, atau dropout.
```

## Data
```Dataset didapatkan dari kaggle yang berisi mengenai data mahasiswa dilihat dari latar belakang keluarga, pendidikan sebelumnya, dan faktor eksternal yaitu ekonomi. Dataset berisi 35 kolom dengan satu kolom sebagai target. Terdapat 17 kolom kategorikal dan sisanya numerik.

Penjelasan kolom kategorikal:
1. Marital status, the marital status of the student: 1. Single, 2. Married, 3. Widower, 4. Divorced, 5. Facto union, 6. Legally separated
2. Application mode, the method of application used by the student: 1. General contingent, 2. Ordinance, 5. Special contingent, 7. Holders of other higher courses, 10. Ordinance No. 854-B/99, 15. International student (Bachelor), 16. Special contingent (Madeira Island), 17. General Contingent, 18. General Contingent, 26. Ordinance No. 533-A/99, 27. Ordinance No. 533-A99, 39. Over 23 years old, 42. Transfer, 43. Change of course, 44. Technological Diploma, 51. CHange of Institution, 53. Short cycle diploma holders, 57. Change of institution/course
3.Course, the course taken by student: 1. Manajemen, 2. Kedokteran, 3. Teknik Mesin, 4. Administrasi Bisnis, 5. Perawat, 6. Ilmu komunikasi, 7. Jurnalistik, 8. Pendidikan biologi, 9. Pendidikan kimia, 10. AKuntansi, 14. Gizi, 17. Hubungan Internasional, 19. Teknik telekomunikasi, 33. Biofuel technology, 171. Animation and multimedia design
4. Daytime/evening attendance, whether the student attends classes during the day or in the evening. 1. Daytime, 0. Evening 
5. Previous qualification, the qualification obtained by the student before enrolling in higher education: 1. Secondary education, 2. Higher education (Bachelor degree), 3. Higher education (Degree), 4. Higher education (Master), 5. Higher education (Doctorate), 6. Frequency of higher education, 9. 12th year of schooling, 10. 11th year of schooling, 38. Basic education, 40. Higher education (degree 2nd), 43. Higher education (Master 2nd)
6. Nationality, the nationality of the student: 1. Portuguese, 2. German, 6. Spanish, 11. Italian, 13. DUtch, 14. English, 17. Lithuanian, 21. Angolan, 22. Cape Verden, 24. Guinean, 25. Nozambican, 26. Santomean, 32. Turkish, 41. Brazilian, 62. Romanian, 100. Moldova, 101. Mexican, 103. Ukrainian, 105. Russian, 108. Cuban, 109. Colombian.
7. Mother's qualification, the qualification of the student's mother
8. Father's qualification, the qualification of the student's father
9. Mother occupation, The occupation of the student's mother: 1. Directors or Executive Manager, 2. Scientific activities, 3. Technicians, 4. Administrative staff, 5. Public service, 6. Farmer, 7. Skilled worker in industry, 8. Machine operators, 9. Unskilled worker, 10. Armed forces, 11. Armed forces officer.
10. Father's occupation, The occupation of the student's father
11. Displaced, whether the student is a displaced person
12. Educational special needs, whether the student has any special educational needs.
13. Debtor, whether the student is a debtor
14. Tuition fees up to date, whether the student's tuition fees are up to date
15. Gender, the gender of the student
16. Scholarship holder, whether the student is a scholarship holder
17. International, whether the student is an international student

Penjelasan kolom numerik:
1. Application order, the order in which student applied, from 0-9
2. Age at enrollment, the age of the student at the time of enrollment
3. Curricular units 1st sem (credited): The number of curricular units credited by the student in the first semester.
4. Curricular units 1st sem (enrolled): The number of curricular units enrolled by the student in the first semester.
5. Curricular units 1st sem (evaluations): The number of curricular units evaluated by the student in the first semester.
6. Curricular units 1st sem (approved): The number of curricular units approved by the student in the first semester.
7. Curricular units 1st sem (credited): The number of curricular units credited by the student in the first semester.
8. Curricular units 1st sem (enrolled): The number of curricular units enrolled by the student in the first semester.
9. Curricular units 1st sem (evaluations): The number of curricular units evaluated by the student in the first semester.
10. Curricular units 1st sem (approved): The number of curricular units approved by the student in the first semester
```

## Method
```
Project machine learning ini menggunakan 5 model, yaitu KNN, SVM, Decision Tree, Random Forest, dan Gradient Boosting. Dari kelima model tersebut akan dicari model terbaik untuk disimpan dan digunakan pada tahap inference.
```

## Stacks
```
Proses machine learning ini diolah di google colab dengan menggunakan python. Libraries yang digunakan yaitu pandas, matplotlib, scipy, sklearn, numpy, feature engine, seaborn, streamlit, json, dan pickle.
```

## Reference
```
URL: https://www.kaggle.com/datasets/thedevastator/higher-education-predictors-of-student-retention
```