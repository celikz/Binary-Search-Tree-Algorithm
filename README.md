# Binary-Search-Tree-Algorithm

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Öncelikle Binary Search Tree algoritmasının nasıl çalıştığına bir göz atalım. Bu algoritma kendisine random bir şekilde eleman seçer, bu elemana "root" adı verilir. Daha sonra root referans alınarak ondan küçük elemanlar sola, ondan büyük elemanlar ise sağa doğru dallanır. Bu şekilde dallar oluşturmaya devam ederek bir ağaç yapısı oluştururlar.

Root: ilk eleman olan 7 kabul edelim.

Sırasıyla elemanlara baktığımız zaman 7'nin yanında 5 elemanı vardır. Bu iki elemanın ilişkisi 5<7 şeklindedir, böylece 5 elemanı 7'nin sol tarafına dallanma yapmalıdır.

![image](https://user-images.githubusercontent.com/67806354/147416966-bff1a686-1175-4b31-a6e8-cd02ad60615d.png)

Sonraki eleman 1'dir. 1 de 7'den küçüktür ve sol tarafa yerleşecektir. Ancak sol tarafta 5 elemanı da var, bu yüzden 1 elemanı 5 elemanından da küçük olduğu için bu sefer 5'in soluna dallanma yaparak konumlanacaktır.

![image](https://user-images.githubusercontent.com/67806354/147417070-9f013ae1-4c40-4756-a046-8950fba1d18f.png)

4üncü eleman 8. Root ile karşılaştırıldığında ondan büyük olduğunu görürüz. Böylece direkt 7'nin sağ tarafına dallanacaktır.

![image](https://user-images.githubusercontent.com/67806354/147417121-f521fc25-d166-48ca-b3ee-27e71f155407.png)

5inci elemanımız 3. 7'den küçük ve sol tarafta konumlanması gerekir. İlk dalı kontrol ettiği zaman 5 node'u ile karşılaşır ve 5'ten küçüktür. 5'in sol tarafında dallanan bir eleman görür ve bu sefer onu kontrol eder, bu eleman ise 1'di. 3, 1'den büyük olduğu için 1'in sağ tarafında konumlanacaktır.

![image](https://user-images.githubusercontent.com/67806354/147417197-2dfa6b21-15a9-4d82-bc9a-5c75c7dce6a4.png)

6ıncı eleman 6'dır ve 7'den küçüktür. Sol tarafı kontrol ettiği zaman 5 elemanı ile karşılaşır. 5'ten büyük olduğu için onun sağ tarafına doğru dal yaparak yerini alır.

![image](https://user-images.githubusercontent.com/67806354/147417239-f7340b35-f0ac-46b8-8f7b-107037de711e.png)

7inci eleman 0'dır. 7'den ve 7'nin solunda bulunan bütün elemanlardan küçüktür. Böylece en alttaki node'un en soluna dal yapacaktır.

![image](https://user-images.githubusercontent.com/67806354/147417274-5ad33b0d-42f8-42fb-9f34-58f89dbbcfeb.png)

8inci eleman 9'dur. Root olan 7'den büyük olduğu için sağ tarafına konumlanmalıdır. Sağ taraftaki elemanları kontrol ederken ilk adımda 8 elemanı ile karşılaşır. 8'den büyük olduğu için onun sağ tarafına konumlanır.

![image](https://user-images.githubusercontent.com/67806354/147417309-10243f6c-6be4-4a36-9b27-191dab9cd939.png)


9uncu eleman 4'tür. Root kontrolünde küçük olduğunu fark eder ve sol tarafa yönelir. Sol tarafta ilk karşılaştığı node 5'tir. 5'i kontrol ettiği zaman ondan küçük olduğunu fark eder. İlerlediğinde 1 ile karşılaşır ve ondan büyük olduğunu fark eder ama 1 elemanı sağ ve sola dallanma yapmıştır. Böylece 0 ve 3 elemanını kontrol ettiğinde her ikisinden de büyük olduğunu fark edip 3'ün ya da 0'ın sağ tarafına konumlanabilir.

![image](https://user-images.githubusercontent.com/67806354/147417463-1c59245a-9c8e-41f5-990b-6465fa240adb.png)

Son eleman ise 2'dir. Direkt root'un solun yönelir ve kontrol etmeye başlar. 3'e geldiği zaman ondan küçük olduğunu anlar ve hemen soluna konumlanır. Böylece tree'miz oluşmuş olur.

![image](https://user-images.githubusercontent.com/67806354/147417508-79ca31d1-dab7-40b3-b89c-c8f8b393dc33.png)
