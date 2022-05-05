# Not Ortalamasi Hesaplayan Program

* Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın.

## Ödev

* Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.
* **Not : If ve Else kullanılmayacak...**

**Cevap:**
```
import java.util.Scanner;

public class NotHesaplama {
    public static void main(String[] args) {

        int mat, fizik, kimya, turkce, tarih, muzik;

        Scanner input = new Scanner(System.in);

        System.out.print("Matematik notunuzu giriniz= ");
        mat = input.nextInt();

        System.out.print("Fizik notunuzu giriniz= ");
        fizik = input.nextInt();

        System.out.print("Kimya notunuzu giriniz= ");
        kimya = input.nextInt();

        System.out.print("Turkce notunuzu giriniz= ");
        turkce = input.nextInt();

        System.out.print("Tarih notunuzu giriniz= ");
        tarih = input.nextInt();

        System.out.print("Muzik notunuzu giriniz= ");
        muzik = input.nextInt();

        int toplam=(mat + fizik + kimya + turkce + tarih + muzik );
        double ortalama = toplam / 6;
        System.out.println("Ortalamaniz= " + ortalama);

        String sonuc = (ortalama > 60) ? "Sinifi Gectiniz" : "Sinifta Kaldiniz.";
        System.out.println(sonuc);



    }
}


```
