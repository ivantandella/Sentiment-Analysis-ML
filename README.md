# Sentiment Analysis Livin by Mandiri Review on Google Playstore

## Data Aquisition
Data review aplikasi Livin by Mandiri terdiri dari:

- 47814 negative
- 47719 positive
- 31773 neutral


## Preprocessing

- `cleaningText(text)`: menghapus mention, hashtag, RT (retweet), angka, tanda baca, tautan, dan angka, menghilangkan spasi di awal dan akhir teks dan menggantikan karakter newline dengan spasi.

- `casefoldingText(text)`:  mengubah semua karakter dalam teks menjadi huruf kecil.

- `tokenizingText(text)`: membagi teks menjadi daftar kata atau token.

- `filteringText(text)`: menghilangkan kata-kata berhenti dalam teks.

- `stemmingText(text)`: mengubah kata-kata menjadi bentuk dasar.

- `toSentence(list_words)`: menggabungkan daftar kata menjadi kalimat.


## Result

- Logistic Regression - train acc: 0.89, test acc: 0.89
- SVM - train acc: 0.92, test acc: 0.90
- Decision Tree - train acc: 0.95, test acc: 0.86
- Random Forest - train acc: 0.95, test acc: 0.88

## Conclusion
Dari hasil percobaan, dapat disimpulkan bahwa model terbaik diperoleh menggunakan algoritma SVM dengan nilai akurasi pada data uji sebesar 90%. Model Decision Tree dan Random Forest memiliki akurasi train lebih tinggi dari SVM, namun dengan akurasi test yang jauh dibawahnya, sehingga dapat memiliki kecenderungan terjadi overfitting.
