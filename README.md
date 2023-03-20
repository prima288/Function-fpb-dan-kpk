# Function-fpb-dan-kpk
Case Flow: program akan meminta pengguna menginputkan 2 buah angka secara bebas. Kemudian pengguna akan menampilkan nilai FPB dan KPK berdasarkan 2 buah angka yang  telah diinputkan.
Penjelasan bagian dalam script =
Function hitung fpb : 
def fpb(a,b):
    if a<b:
        smaller=a
    else:
        smaller=b
    for i in range (1,smaller+1):
        if a%i==0 and b%i==0:
            fpb=i
        # else:
        #     continue
    return fpb
    
Function hitung kpk :  
kpk=int(a*b/fpb(a,b))
    return kpk

Menginput masukan angka :
a=int(input('Masukkan angka pertama :'))
b=int(input('Masukkan angka kedua   :'))

Menampilkan hasil :
print('FPB dari ',a,' dan ',b,' adalah ',fpb(a,b))
print('KPK dari ',a,' dan ',b,' adalah ',kpk(a,b),'\n')

Output:
Masukkan angka pertama :20
Masukkan angka kedua   :35
FPB dari  20  dan  35  adalah  5
KPK dari  20  dan  35  adalah  140 
