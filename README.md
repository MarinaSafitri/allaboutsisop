allaboutsisop
=============

serba-serbi mata kuliah sistem operasi

Animasi dalam Android

Dalam pembuatan game, Animasi adalah hal yang sangat penting, karena untuk membuat game yang menarik harus memiliki pergerakan. pada tutorial ini penulis akan membuat animasi yang sederhana. bola yang ada dalam canvas akan bergerak terus menerus di dalam gambar. Untuk melakukan pengontrolan agar bola tetap di dalam canvas, penulis gunakan source berikut :


if (x >= getWidth() - gambarBola.getWidth()) {
 xSpeed = -10;
}
if (x == 0) {
 xSpeed = 10;
}
x = x + xSpeed;

if (y >= getHeight() - gambarBola.getHeight()) {
 ySpeed = -10;
}
if (y == 0) {
 ySpeed = 10;
}
y = y + ySpeed;

canvas.drawColor(Color.WHITE);
canvas.drawBitmap(gambarBola, x , y, null);
