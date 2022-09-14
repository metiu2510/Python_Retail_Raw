# Python_Retail_Raw

Diberikan dataset ‘retail_raw_test.csv’

Baca dataset
Tipe data diubah menjadi tipe yang seharusnya
customer_id dari string ke int64,
quantity dari string ke int64,
item_price dari string ke int64
transform product_value supaya bentuknya seragam dengan format PXXXX, assign ke kolom baru "product_id", dan drop kolom "product_value", jika terdapat nan gantilah dengan "unknown".
trasnform order_date menjadi value dengan format YYYY-mm-dd
cek data hilang dari tiap kolom dan kemudian isi missing value
di brand dengan "no_brand", dan
cek dulu bagaimana missing value di city & province - isi missing value di city dan province dengan "unknown"
create column city/province dari gabungan city & province
membuat index berdasarkan city_provice, order_date, customer_id, order_id, product_id (cek index)
membuat kolom "total_price" sebagai hasil perkalian quantity dengan item_price
slice data hanya untuk Jan 2019
