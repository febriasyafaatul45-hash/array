# 
// 1. Buat array isinya angka acak
let angka = [];

for (let i = 0; i < 10; i++) {
    angka.push(Math.floor(Math.random() * 100) + 1);
}

console.log("Array awal:", angka);

// 2. Urutkan dari terbesar ke terkecil
let terbesar = [...angka].sort((a, b) => b - a);
console.log("Terbesar ke terkecil:", terbesar);

// 3. Urutkan dari terkecil ke terbesar
let terkecil = [...angka].sort((a, b) => a - b);
console.log("Terkecil ke terbesar:", terkecil);

// 4. Jumlahkan semua nilai dalam array
let jumlah = angka.reduce((total, nilai) => total + nilai, 0);
console.log("Jumlah semua angka:", jumlah);

// 5. Tampilkan angka genap saja (angka ganjil tidak ditampilkan)
let genap = angka.filter(nilai => nilai % 2 === 0);
console.log("Angka genap saja:", genap);
