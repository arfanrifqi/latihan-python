# latihan-soal-python

# Buat program yang mencetak seluruh bilangan prima yang lebih kecil dari 100

def is_prima (x):
  for i in range(2, x):
    if x % i == 0:
        return False
    
  return True

def cari_bilangan_prima (awal, akhir):
    list_bilangan_prima = []
    for x in range(awal, akhir + 1):
        if is_prima(x):
            list_bilangan_prima.append(x)
    return list_bilangan_prima

print(cari_bilangan_prima(1, 100))
