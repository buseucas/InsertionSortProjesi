# **[22,27,16,2,18,6] -> Insertion Sort**
### 1.	Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
### 2.	Big-O gösterimini yazınız.
### 3.	Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
### 4.	Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

---

## **Cevap 1:**
### **AŞAMA 1: [22,27,16,2,18,6] ----> [2,27,16,22,18,6]**
### **AŞAMA 2: [2,27,16,22,18,] ----> [2,6,16,22,18,27]**
### **AŞAMA 3: [2,6,16,22,18,27] ----> [2,6,16,18,22,27]**

---

## **Cevap 2:**
### **AŞAMA 1: [22,27,16,2,18,6] ----> [2,27,16,22,18,6] --> n**
### **AŞAMA 2: [2,27,16,22,18,6] ----> [2,6,16,22,18,27] --> n-1**
### **AŞAMA 3: [2,6,16,22,18,27] ----> [2,6,16,18,22,27] --> n-2**
## ***n.(n+1)÷2=n2+n÷2= O(n2)***

---

## **Cevap 3:**
* Worst case: Aradığımız sayının sonda olması.

Tam ters verilmiş dizi, bu durumda dizinin her bir elemanı bir gerisindekinden küçük olacaktır. Dolayısıyla 1inci eleman için iç döngü 0 2 eleman için geriye doğru 1, 3. eleman için iki daha sonra 3 4 5 6… n kadar geriye hareket yapacaktır. Yani 0+1+2+3+4…..+n-1 = [n*(n-1)]/2 : n^2

* Average case: Aradığımız sayının ortada olması.

Worst case ile best casein ortalamasını aldığımızda n^2 olarak buluruz.
* Best case: Aradığımız sayının dizinin en başında olması.

Tam sıralı dizi, n tane sayinin üzerinden birer defa geçer ve hiç birini geriye doğru ilerletme gereği 
olmadığı için bu tek geçişle kalır. Yani n.

---

## **Cevap 4:**
Average case kapsamına girer.

---

**[7,3,5,8,2,9,4,15,6]** dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

## **Cevap:**

**AŞAMA 1: [7,3,5,8,2,9,4,15,6] ----> [2,3,5,8,7,9,4,15,6]**

**AŞAMA 2: [2,3,5,8,7,9,4,15,6] ----> [2,3,4,8,7,9,5,15,6]**

**AŞAMA 3: [2,3,4,8,7,9,5,15,6] ----> [2,3,4,5,7,9,8,15,6]**

**AŞAMA 4: [2,3,4,5,7,9,8,15,6] ----> [2,3,4,5,6,9,8,15,7]**