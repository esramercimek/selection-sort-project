# selection-sort-project


**[22,27,16,2,18,6] -> Insertion Sort**

**I) Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.**

solution ==> 
1. [22,27,16,2,18,6] (n) (2 en küçük olduğu için en başa geçerek 22 ile yer değiştirir)
2. [2,27,16,22,18,6] (n-1) (sıradaki en küçük sayı 6 olduğu için 27 ile yer değiştirerek 2. sıraya yerleşir)
3. [2,6,16,22,18,27] (n-2) (16dan sonra gelen küçük sayı 18 olduğu için 22 ile yer değiştirerek 4. sıraya yerleşir)
4. [2,6,16,18,22,27]   1   (sorting gerçekleştirildi)

```

**II) Big O gösterimini yazınız.**

solution ==>  
n+(n-1)+(n-2)+...+1=(n*(n+1))/2=((n²)+n)/2 olur. Big-O'da kat sayı önemsizdir. Domine eden fonksiyon n² alınır. Big O değerimiz O(n²)'dir.

```

**III) Time Complexity: Dizi sıralandıktan sonra 18 sayısı case'lerden hangisinin kapsamına girer? Yazınız.**

solution ==> 
insertion sorting ile elde ettiğimiz sonuçta [2,6,16,18,22,27] 18 ortada olduğu için avergae case kapsamına girer.

```

**IV) [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.**

solution ==>
1. adım: en küçük 2 olduğu için ilk sıraya 2 yazarak 7 ve 2'nin yerini değiştiririz. [2,3,5,8,7,9,4,15,6]
2. adım: sıradaki küçük sayı 3 olduğu için yerini korur, 4 rakamı 3 ile 5 arasına yerleştirilir. [2,3,4,5,8,7,9,15,6]
3. adım: 5'ten sonra en küçük rakam 6 olduğundan 5 ve 8'in arasına yerleşir. [2,3,4,5,6,8,7,9,15]
4. adım: son olarak 7 rakamı 6 ve 8 arasına yerleşir. [2,3,4,5,6,7,8,9,15]
