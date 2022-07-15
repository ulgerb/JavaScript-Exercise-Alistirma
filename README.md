# JavaScript-Exercise-Al-t-rma
JavaScript Exercise || Example || Alıştırma ||Örnekler
JavaScript Methot || DOM || Properties || Array || Object || Function || Filter 

-Yakında DOM ve diğer methotlarda eklenicek.
-Python, C++ için de oluştumayı düşünüyorum.


    var arr1 = [1,2,3,4,6,5];
    var arr2 = ["a", "b", "g", "c", "y", "k", "c"]
    var array1 = ["bir", "iki",1,2,4,3,"1"];
    var array2 = ["iki",1,3,1, "üç"];
    var arra = "selam" 
    
    // ALIŞTIRMALARI SIRASIYLA YORUMDAN ÇIKARARAK DENEYEBİLİRSİNİZ
    
    //*******************************************************
    //===== push() arrayin sonuna eleman ekle =====
    //arr1.push("2");
    //console.log(arr1);//[1, 2, 3, 4, 6, 5, '2'];

    //*******************************************************
    //===== unshift() arrayin başına eleman ekle =====
    //arr1.unshift(7);
    //console.log(arr1);//[7, 1, 2, 3, 4, 6, 5]

    //*******************************************************
    //===== pop() arrayin son elemanını sil =====
    //arr1.pop();
    //console.log(arr1);//[1, 2, 3, 4, 6];

    //*******************************************************
    //===== shift() arrayin ilk elmanını sil =====
    //arr1.shift();
    //console.log(arr1);//[2, 3, 4, 6, 5]

    //*******************************************************
    //===== splice(index,çıkart,eleman1,eleman2) array indexine eleman ekle & çıkar =====
    //arr1.splice(2,1,5,"muz")
    //console.log(arr1);//[1, 2, 5, 'muz', 4, 6, 5] 

    //*******************************************************
    //===== length arrayin uzunluğunu bulur =====
    //leng = arr1.length
    //console.log(leng);//6

    //*******************************************************
    //===== toString() arrayi stringe dönüştür =====
    //text = arr1.toString();
    //console.log(text);//1,2,3,4,6,5

    //*******************************************************
    //===== Array.from() yapıyı arraye dönüştürür =====
    //console.log(Array.from(arra));//[s, e, l, a, m]

    //*******************************************************
    //===== Array.isArray() array olup olmadığını kontrol eder =====
    //console.log(Array.isArray(arr1));//true
    
    //*******************************************************
    //=====  =====

    //*******************************************************
    //===== map (Harita) =====
    //const mapped1 = arr1.map(element => element + 30);
    //const mapped2 = arr1.map(Math.sqrt);
    //console.log(mapped1);
    //console.log(mapped2);

    //*******************************************************
    //===== filtre (seçici) =====
    //const filtreleme = arr1.filter(element => element ===3 || element === 4);
    //console.log(filtreleme);

    //*******************************************************
    //===== sort(sıralama) & reverse(tersi)  |NOT: arr1 bağlı tüm arraylari de değiştirir!! =====
    //siralama = arr1.sort((a,b) => a < b ? -1:1);
    //siralama = arr1.sort((a,b) => a - b);
    //siralama = siralama.reverse()
    //console.log(siralama);

    //*******************************************************
    //===== forEach(elem, index, array) (eleman gezici) =====
    //arr1.forEach((elem,index,array) => {
    //    console.log("element", elem,"index", index,"list", array);
    //})
    //===== 2. yol =====
    //myFunc = (elem, index, array)  => {return array[index] = elem * 10}
    //arr1.forEach(myFunc)
    //console.log(arr1);
    
    //*******************************************************
    //===== concat() (2 arrayi birleştirme, metin birleştirmek içinde kullanılır) =====
    //arr1arr2 = arr1.concat(arr2)
    //arr1arr2 = [arr2 +["",""]+ arr1]
    //arr1arr2 = [...arr1 ,...arr2]
    //console.log((arr1arr2));//arr1+arr2
    
    //*******************************************************
    //============ set(ayarlamak) tüm kopyaları kaldırır =============
    //======= array içindeki tekrarları sil ve topla ========
    //var array3 = array1.concat(array2)
    //const union = Array.from(new Set([...array1, ...array2]));
    //const union = [...new Set(array3)];
    //console.log(union);// ["bir","iki", 1, 2, 4, 3, "1", "üç"]
    //===== 2.yol =====
    //var array4 = array3.filter((item, pos) => array3.indexOf(item) === pos)
    //console.log(array4) // ["bir","iki", 1, 2, 4, 3, "1", "üç"]

    //*******************************************************
    //===== every(her) koşulu elemanların hepsi sağlıyorsa true,biri bile yoksa false =====
    //everyBoole = arr1.every(item => item > 5) //false
    //everyBoole = arr1.every((item,index,array) => index < 6) //true
    //console.log(everyBoole);
    //const isSubset = (array1, array2) => array2.every(element => array1.includes(element));

    //*******************************************************
    //===== some(bazen) koşulu elemanların biri bile sağlıyorsa true,hiç yoksa false döndürür =====
    //someBoole = arr1.some(item => item > 5)//true
    //someBoole = arr1.some(item => item < 0)//false
    //console.log(someBoole);

    //*******************************************************
    //===== includes(içerir) istenilen değer arrayin içinde varsa true, yoksa false  =====
    //includesBoole = arr1.includes(3)//true
    //includesBoole = arr1.includes(8)//false
    //console.log(includesBoole);

    //*******************************************************
    //===== join("") elemanları birleştirir =====
    //joinArr = arr1.join("")
    //console.log(joinArr);//123465
    
    //*******************************************************
    //===== reduce() tüm değerleri toplar yada çarpar =====
    //reduceArr = arr1.reduce((a, b) => a + b);
    //console.log(reduceArr);
    
    //**************** Bulma Metotları *******************
    //*******************************************************
    //===== find(bulma) koşulu sağlayan ilk elementi döndürür =====
    //findArr = arr1.find(item => item > 4)
    //console.log(findArr);//6

    //*******************************************************
    //===== findIndex() koşulu sağlayan ilk elementin indexini döndürür =====
    //findIndexArr = arr2.findIndex(item => item > "c")
    //console.log(findIndexArr);//2

    //*******************************************************
    //===== indexOf() elementin ilk indexini bul  =====
    //indexArr = arr2.indexOf("c")
    //console.log(indexArr);//3
    //*******************************************************
    //===== lastIndexOf() elementin son indexini bul  =====
    //var indexx = arr2.lastIndexOf("c", 3);
    //indexArr = arr2.lastIndexOf("c")
    //console.log(indexArr);//6
    
    //*******************************************************
    //===== search(/text/gi) metin içinde arama yapar =====
    //var metin = "Merhaba ben Berkay ÜLGER";
    //console.log(metin.search(/berkay/gi));

    //*******************************************************
    //===== fill(doldurma) elementler statik olur ve girilen sayıyı döndürür =====
    //arr3 = new Array(4);
    //console.log(arr3.fill(3));//[3, 3, 3, 3]
    //console.log(arr1.fill(5));//[5, 5, 5, 5, 5, 5]
    
    //******************************,*************************
    //===== slice(dilim) iki index arasındaki elemanları döndürür =====
    //sliced = arr1.slice(1,5)
    //console.log(sliced);//[2, 3, 4, 6]
    
    //&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
    //********************* String **************************

    //*******************************************************
    //===== toString(num) string dönüştürme |NOT:num=sayı tabanına dönüştürür =====
    //console.log(typeof (arr1));//object,array
    //console.log(arr1);//[1, 2, 3, 4, 6, 5]
    //var str1 = arr1.toString();
    //console.log(typeof(str1));//string
    //console.log(str1);//1,2,3,4,6,5

    //*******************************************************
    //===== trim() boşlukları kaldır |NOT:başlangıç ve bitiş =====
    //var metin = "           Merhaba     ben javascript öğreniyorum      ";
    //console.log(metin.trim());//Merhaba     ben javascript öğreniyorum
    //console.log(metin.replace(/^\s+|\s+$/gm,''));//Merhaba     ben javascript öğreniyorum

    //*******************************************************
    //===== substring(num,num) belirli aralıktaki metni alır =====
    //var metin = "Merhaba ben Berkay ÜLGER";
    //console.log(metin.substring(12, 24));//Berkay ÜLGER

    //*******************************************************
    //===== substr(num,num) başlangıç,karakter sayısı içini döndürür =====
    //var metin = "Merhaba ben Berkay ÜLGER";
    //console.log(metin.substr(12,12));//Berkay ÜLGER

    //*******************************************************
    //===== replace(str, str)<yer değiştirmek> yazıyı başka yazıyla değiştirir |NOT: büyük küçük harf duyarlıdır =====
    //var metin = "Merhaba ben Basri ÜLGER";
    //console.log(metin.replace("Basri", "Berkay"));//Merhaba ben Berkay ÜLGER

    //*******************************************************
    //===== charAt(num) girilen indexteki karakteri döndürür =====
    //var metin = "Merhaba ben javascript öğreniyorum";
    //console.log(metin.charAt(6));//a
    //*******************************************************
    //===== charCodeAt(num) girilen indexteki karakterin codunu döndürür =====
    //var metin = "Berkay";
    //console.log(metin.charCodeAt(0));//66
    //*******************************************************
    //===== fromCharCode(num,num...) girilen sayı codelarını dönüştürür =====
    //console.log(String.fromCharCode(66,101,114,107,97,121));

    //*******************************************************
    //===== split(str)<bölmek> stringi array içindeki elemanlara dönüştürür =====
    //var metin = "Berkay ÜLGER";
    //console.log(metin.split(" "))//['Berkay', 'ÜLGER']
    //console.log(metin.split(""))//['B','e','r','k','a','y',' ','Ü','L','G','E','R']
    //console.log(metin.split(r))//['Be', 'kay ÜLGER']
    
    //*******************************************************
    //===== endsWith(str,num) son karakteri kontrol eder true ve false döndürür ,girilen sayıyı yazının son karakter kabul eder =====
    //var metin = "Merhaba ben javascript öğreniyorum";
    //console.log(metin.endsWith("yorum"));//true
    //*******************************************************
    //===== startsWith() ilk karakteri kontrol eder true,false döndürür, girilen sayı yazının ilk karakter kabul eder =====
    //var metin = "Merhaba ben javascript öğreniyorum";
    //console.log(metin.startsWith("Merha"));//true

    //*******************************************************
    //===== str1.localeCompare(str2) str2 harf sırası önde=1, geride=-1, eşit=0 =====
    //metin1="Beyaz";
    //metin2="Berkay";
    //console.log(metin1.localeCompare(metin2));//1

    //*******************************************************
    //===== toLowerCase() yazıyı küçült =====
    //var metin = "Berkay ÜLGER";
    //console.log(metin.toLowerCase());//berkay ülger
    //*******************************************************
    //===== toUpperCase() yazıyı büyüt =====
    //var metin = "Berkay Ülger";
    //console.log(metin.toUpperCase());//BERKAY ÜLGER
    
    //*******************************************************
    //===== valueOf() genelde çağırma işlemlerinde kullanılır =====
    //var metin = "javascript öğreniyorum";
    //console.log('text.valueOf(); ', metin.valueOf());




    //&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
    //********************** Date() ************************

    //*******************************************************
    //===== new Date(year, month, day, hours, minutes, seconds, milliseconds); =====
    //console.log(new Date(2018, 11, 24, 10, 33, 30, 0));//Mon Dec 24 2018 10:33:30 GMT+0300 (GMT+03:00)
    //console.log(Date(2018, 11, 24, 10, 33, 30, 0));//== new Date() 
    
    //*******************************************************
    //===== Date() methotları =====
    //console.log(new Date().getHours());//hourse
    //console.log(new Date().getDate());//day 1..31
    //console.log(new Date().getFullYear());//year
    //console.log(new Date().toDateString());//Wed Jul 06 2021
    
    
