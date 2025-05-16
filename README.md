> How much data your publisher program will send to the message broker in one
run?

Didalam fungsi main dalam program publisher terdapat 5 kali panggilan fungsi `publish_event`, sehingga yang terkirim adalah 5 pesan.

>  The url of: *amqp://guest:guest@localhost:5672* is the same as in the subscriber program, what does it mean?

Hal ini berarti bahwa lokasi URL broker yang dipakai publisher (client yang ingin mengirim pesan) sama dengan yang dipakai subscriber (client yang ingin menerima pesan). Hal ini agar broker yang dipakai sama, sehingga pesan dapat dikirim dan diterima.