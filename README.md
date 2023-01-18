Ini adalah aplikasi Android yang menggunakan perpustakaan IntentIntegrator untuk memindai kode QR. Aplikasi ini dapat menangani berbagai jenis kode QR, seperti nomor telepon, URL, alamat email, dan data JSON. Ketika kode QR dipindai, aplikasi memeriksa isinya dan melakukan tindakan yang sesuai, seperti melakukan panggilan telepon, membuka halaman web, mengirim email, atau menampilkan data JSON di layar. Aplikasi juga menampilkan pesan jika kode QR tidak dipindai atau jika kode QR yang dipindai tidak dalam format yang dikenali./
pertama saya akan menjelaskan pembacaan data JSON (java script object notain ) berikut adalah codenya/
```                JSONObject jsonObject = new JSONObject(result.getContents());
                textViewName.setText(jsonObject.getString("nama"));
                textViewClass.setText(jsonObject.getString("kelas"));
                textViewID.setText(jsonObject.getString("nim"));

            }  catch (JSONException e){
                e.printStackTrace();
                Toast.makeText(this, result.getContents(), Toast.LENGTH_LONG).show();
            }

            Toast.makeText(this, "Scanned : " + result.getContents(), Toast.LENGTH_LONG).show();
        }
    }


berikut ini adalah gambar QR yang saya buat untuk praktek projek JSON

```