// Tunggu hingga halaman selesai dimuat sepenuhnya
document.addEventListener("DOMContentLoaded", function() {
    // Cari elemen canvas di HTML
    const ctx = document.getElementById('stuntingChart').getContext('2d');

    // Data Stunting dari Tahun ke Tahun
    const tahun = ['2020', '2021', '2022', '2023', '2024', '2025', '2026'];
    const dataJumlahKasus = [45, 38, 29, 22, 15, 9, 4]; // Contoh jumlah balita stunting

    // Konfigurasi Chart.js
    const stuntingChart = new Chart(ctx, {
        type: 'bar', // Menggunakan tipe Bar Chart (grafik batang) seperti referensi gambar Anda
        data: {
            labels: tahun,
            datasets: [
                {
                    label: 'Jumlah Kasus Stunting',
                    data: dataJumlahKasus,
                    backgroundColor: 'rgba(45, 122, 95, 0.85)', // Warna hijau sage seperti di gambar
                    borderColor: '#2d7a5f',
                    borderWidth: 1.5,
                    borderRadius: 6, // Membuat ujung atas batang agak melengkung manis
                    borderSkipped: false,
                    barPercentage: 0.6 // Mengatur ketebalan batang agar tidak terlalu rapat
                }
            ]
        },
        options: {
            responsive: true,
            maintainAspectRatio: false,
            plugins: {
                legend: {
                    position: 'top',
                    labels: {
                        color: '#2c3e50',
                        font: {
                            weight: '600'
                        }
                    }
                },
                tooltip: {
                    callbacks: {
                        label: function(context) {
                            return ` ${context.dataset.label}: ${context.raw} Anak`;
                        }
                    }
                }
            },
            scales: {
                y: {
                    beginAtZero: true,
                    grid: {
                        color: '#f0f3f4'
                    },
                    ticks: {
                        color: '#7f8c8d',
                        stepSize: 10
                    },
                    title: {
                        display: true,
                        text: 'Jumlah Kasus (Anak)',
                        color: '#7f8c8d'
                    }
                },
                x: {
                    grid: {
                        display: false // Hilangkan garis vertikal agar grafik terlihat bersih seperti gambar referensi
                    },
                    ticks: {
                        color: '#7f8c8d'
                    }
                }
            }
        }
    });
});