# Proyek-Mandiri

Merupakan reproduce code dari Paper "Knowledge Enriche Transformer for Emotion Detection in Textual Conversation" oleh Peixiang Zhong, Di Wang dan Chunyan Miao". Paper dapat diakses di https://www.aclweb.org/anthology/D19-1016.pdf .

File terdiri dari :
1. File preProcessData.ipynb , untuk memproses data train, test dan val dari datsaet DailyDialogues (DD) ke dalam format pkl
2. File preProcessCN.ipynb , untuk memproses data Conceptnet dan NRC VAD (knowledge Representation) dan menyimpannya dalam format pkl
3. File train4.ipynb untuk proses training model
4. File hasil1.txt berupa hasil dari percobaan pertama. Disini dicoba 30 epoch, berhenti pada epoch ke-27 (maksimal runtime)
   hasil terbaik ada pada epoch ke-8
5. File hasil2.txt berupa hasil percobaan kedua. Menggunakan checkpoint dari epoch ke-8 dari hasil percobaan pertama ; dan disertai dengan perubahan hyperparameter.
   Dicoba dengan 10 epoch, hasil terbaik pada epoch ke-2.  
   
Folder "data" :
Berisi dataset Daily Dailogues (DD) : versi gabungan dan versi split data menjadi train, validation dan test

Folder 'explore'
Untuk explorasi dengan dataset yang sama menggunakan RoBERTa, tanpa unsur knowledge representation
Berisi file :
1. File preProcessSimpleTrans.ipynb : untuk preproses data menjadi bentuk yang siap untuk digunakan pada RoBERTa
2. File SimpleTransformer.ipynb : untuk train dan validation model RoBERTa 
