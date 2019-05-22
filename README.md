# backup-bpmn

# Cara Penggunaan : 
1. Download & Extract
2. Pergi ke dalam folder backup-bpmn > cmd 
3. Ketik code ini
```
npm install
```
4. Setelah selesai 
```
cd app
npm install
```
5. Untuk penggunaan Google Drive : Code editor  -> backupbpmn/app/src/component/pages/BpmnModelerComponent.js dan /BpmnModelerDemo.js.
Kemudian, Find function initClient() dan ubah Client ID beserta API KEY pada bagian code dibawah
```
window.gapi.client.init({
          'apiKey': '{API KEY / Developer Key}',
          'discoveryDocs': [discoveryUrl],
          'clientId': '{Client ID Key}',
          'scope': SCOPE
      })
```
6. Pergi ke backupbpmn/app/src/component/pages/project.js
Find Google Picker dan lakukan pengubahan API KEY dan Client ID seperti langkah ke 5 
```
<button type="button" id="getDrive"><GooglePicker clientId={'Client ID'}
                        developerKey={'APIKey'}
```
7. Aplikasi siap untuk digunakan dengan kembali ke dalam folder backup-bpmn > cmd > npm run dev untuk menjalankan server node dan react

# NB :
jangan lupa untuk melakukan install mongoDB dan Robo 3T(opsional untuk melihat isi database)
