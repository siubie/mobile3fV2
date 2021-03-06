#Rangkuman Pertemuan 04 - ListView & RecyclerView


List View

- Dalam pengembangan Android, setiap kali kami ingin menampilkan daftar vertikal item yang dapat digulir, kami akan menggunakan LisView yang memiliki data yang diisi menggunakan Adaptor
- Adaptor paling sederhana untuk digunakan disebut ArrayAdapter karena adaptor mengonversi objek ArrayList menjadi item View yang dimuat ke dalam container ListView.

ArrayAdapter

ArrayAdapter<String> itemsAdapter = 
    new ArrayAdapter<String>(this, android.R.layout.simple_list_item_1, items);

ListView listView = findViewById(R.id.lvItems);
listView.setAdapter(itemsAdapter);

Custom ArrayAdapter

- Define the Model
- Create View Template
- Define the Adapter -> ArrayAdapter Inheritance
- Attaching the Adapter to a ListView
- Populating Data into ListView

RecyclerView

- RecyclerView adalah ViewGroup yang merender tampilan berbasis adaptor dengan cara yang serupa. Itu seharusnya menjadi penerus ListView dan GridView.
- Setiap elemen individu dalam daftar ditentukan oleh objek view holder. Anda menentukan view holder dengan memperluas RecyclerView.ViewHolder.
- RecyclerView meminta tampilan tersebut, dan mengikat tampilan ke datanya, dengan memanggil metode di adaptor. Anda menentukan adaptor dengan memperluas RecyclerView.Adapter.
- Manajer tata letak mengatur elemen individual dalam daftar Anda. Anda dapat menggunakan salah satu pengelola tata letak yang disediakan oleh pustaka RecyclerView, atau Anda dapat menentukan sendiri. Manajer tata letak semuanya didasarkan pada kelas abstrak LayoutManager perpustakaan.

LayoutManagers

RecyclerView menyediakan pengelola tata letak bawaan ini:
- LinearLayoutManager menampilkan item dalam daftar gulir vertikal atau horizontal.
- GridLayoutManager menampilkan item dalam kotak.
- StaggeredGridLayoutManager menampilkan item dalam kisi terhuyung.

Adapter

- RecyclerView menyertakan jenis adaptor baru. Ini adalah pendekatan yang mirip dengan yang sudah Anda gunakan, tetapi dengan beberapa kekhasan, seperti ViewHolder yang diperlukan.
Anda perlu mengganti tiga metode:
- onCreateViewHolder()
- diBindViewHolder()
- getItemCount()
