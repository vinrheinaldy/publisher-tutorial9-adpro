<details> <summary>a. How much data your publisher program will send to the message broker in one run?</summary>

Program publisher mengirim 5 pesan ke message broker dalam satu kali eksekusi. Setiap pesan berupa `UserCreatedEventMessage` yang berisi informasi user sebagai berikut:
1. `user_id: "1", user_name: "2306275866-Amir"`
2. `user_id: "2", user_name: "2306275866-Budi"`
3. `user_id: "3", user_name: "2306275866-Cica"`
4. `user_id: "4", user_name: "2306275866-Dira"`
5. `user_id: "5", user_name: "2306275866-Emir"`

</details> <details> <summary>b. The url of “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?</summary>

URL "amqp://guest:guest@localhost:5672" adalah URL koneksi AMQP (Advanced Message Queuing Protocol) dengan komponen sebagai berikut:
- Protocol: amqp
- Username: guest
- Password: guest
- Host: localhost
- Port: 5672

Penggunaan URL amqp://guest:guest@localhost:5672 yang sama di publisher dan subscriber menunjukan bahwa publisher dan subscriber terhubung ke instance message broker yang sama. Hal ini diperlukan agar message broker dapat menerima pesan dari publisher dan mengirimkannya ke subscriber. Dengan kata lain, keduanya harus terhubung ke broker yang sama agar dapat berkomunikasi.

</details>


### RabbitMQ running in localhost
![rabbitmqrunning](image/rabbitmqrunning.png)
