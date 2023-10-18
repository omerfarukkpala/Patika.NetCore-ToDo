# Patika.NetCore101-ToDo
Console ToDo Application


![boardlisteleme](https://user-images.githubusercontent.com/101570820/161508563-7d945e0d-d510-4739-8e72-f4bdef1828e7.jpg)
![4-karttasima](https://user-images.githubusercontent.com/101570820/161508570-5d72a9c2-1d8c-4d61-8a22-93c76a259ddc.jpg)
![3-kartsilme](https://user-images.githubusercontent.com/101570820/161508574-57f0fa3f-1ef4-4ed0-a8aa-067e31322507.jpg)
![2-boardkartekleme](https://user-images.githubusercontent.com/101570820/161508575-ef7128cd-c811-422e-951a-a1435cb3c05e.jpg)

Kart Ekle
Kart Güncelle
Kart Sil
Kart Taşı
Board Listeleme


# Kart İçeriği:



Baslık
Icerik
Atanan Kisi (Takım üyelerişnden biri olmalı)
Büyüklük (XS, S, M, L, XL)


Açıklama:

Board TODO - IN PROGRESS - DONE kolonlarından oluşmalı.


Varsayılan olarak bir board tanımlı olmalı ve 3 tane de kart barındırmalı.(Kartlar herhangi bir line'da yani kolonda olabilir.)


Kartlar ancak takımdan birine atanabilir. Takımdaki kişiler ise varsayılan olarak tanımlanmalı. Takım üyeleri Dictionary kullanılarak key-value pair şeklinde yada bir sınıf aracılığıyla tutulabilir. Kartlara atama yapılırken takım üyeleri ID leri ile atanacak. Yani kullanılacak ypının mutlaka bir ID içermesi gerekir.


Uygulama ilk başladığında kullanıcıya yapmak istediği işlem seçtirilir.

  Please choose the action you want to perform:
*******************************************
(1) List Boards
(2) Add Card to Board
(3) Delete Card from Board
(4) Move Card



(1) Board Listelemek


 TODO Line
 ************************
 Başlık      :
 İçerik      :
 Atanan Kişi :
 Büyüklük    :
 -
 Başlık      :
 İçerik      :
 Atanan Kişi :
 Büyüklük    :
 
 
 IN PROGRESS Line
 ************************
 Başlık      :
 İçerik      :
 Atanan Kişi :
 Büyüklük    :
 -
 Başlık      :
 İçerik      :
 Atanan Kişi :
 Büyüklük    :


 DONE Line
 ************************
 ~ BOŞ ~


(2) Board'a Kart Eklemek


 Başlık Giriniz                                  : 
 İçerik Giriniz                                  :
 Büyüklük Seçiniz -> XS(1),S(2),M(3),L(4),XL(5)  :
 Kişi Seçiniz                                    : 
**Büyüklükler Enum olarak saklanmalı. Kart üzerinde gösterilirken XS olarak gösterilmeli. Giriş yapılırken kullanıcıdan 1 alınmalıdır.



**Takım üyeleri mevcut bir listede daha tanımlanmış olamlıdır.(Program içerisinde dinamik tanımlanmasına gerek yok.) Kart tanımlarken takım üyesinin ID'si istenmeli. Tanımlı bir ID değilse "Hatalı girişler yaptınız!" uyarısı ile işlem iptal edilebilir.



(3) Board'a Kart Silmek


 Öncelikle silmek istediğiniz kartı seçmeniz gerekiyor.
 Lütfen kart başlığını yazınız:  


Kart bulunamaz ise:



 Aradığınız krtiterlere uygun kart board'da bulunamadı. Lütfen bir seçim yapınız.
 * Silmeyi sonlandırmak için : (1)
 * Yeniden denemek için : (2)
** Aynı isimde birden fazla kart bulunursa her ikisi de silinebilir.



(4) Kart Taşımak


 Öncelikle silmek istediğiniz kartı seçmeniz gerekiyor.
 Lütfen kart başlığını yazınız:  


Kart bulunamaz ise:



 Aradığınız krtiterlere uygun kart board'da bulunamadı. Lütfen bir seçim yapınız.
 * İşlemi sonlandırmak için : (1)
 * Yeniden denemek için : (2)


Kart bulunur ise:



 Bulunan Kart Bilgileri:
 **************************************
 Başlık      :
 İçerik      :
 Atanan Kişi :
 Büyüklük    :
 Line        :

 Lütfen taşımak istediğiniz Line'ı seçiniz: 
 (1) TODO
 (2) IN PROGRESS
 (3) DONE
** Doğru bir seçim yapılırsa board listelenerek (1) Board Listelemek kullanılarak kullanıcıya gösterilir. Seçim doğru değil ise "Hatalı bir seçim yaptınız!" bilgisi ile işlem sonlandırılabilir.
# Patika.NetCore101-ToDo
Console ToDo Application

## Screenshots

### List Boards
![List Boards](https://user-images.githubusercontent.com/101570820/161508563-7d945e0d-d510-4739-8e72-f4bdef1828e7.jpg)

### Move Card
![Move Card](https://user-images.githubusercontent.com/101570820/161508570-5d72a9c2-1d8c-4d61-8a22-93c76a259ddc.jpg)

### Delete Card
![Delete Card](https://user-images.githubusercontent.com/101570820/161508574-57f0fa3f-1ef4-4ed0-a8aa-067e31322507.jpg)

### Add Card
![Add Card](https://user-images.githubusercontent.com/101570820/161508575-ef7128cd-c811-422e-951a-a1435cb3c05e.jpg)

## Card Content

- Title
- Content
- Assigned Person (Must be a team member)
- Size (XS, S, M, L, XL)

## Explanation

The board should consist of columns: TODO - IN PROGRESS - DONE.

By default, there should be a predefined board containing 3 cards. (Cards can be in any line/column.)

Cards can only be assigned to a team member. Team members can be defined by using a Dictionary with key-value pairs or through a class. When assigning cards, team members will be assigned with their IDs. Therefore, the structure used must have an ID.

When the application starts, the user should be prompted to choose an action.

```markdown
Please choose the action you want to perform:
*******************************************
(1) List Boards
(2) Add Card to Board
(3) Delete Card from Board
(4) Move Card
TODO Line
************************
Title       :
Content     :
Assigned Person :
Size        :
-
Title       :
Content     :
Assigned Person :
Size        :

IN PROGRESS Line
************************
Title       :
Content     :
Assigned Person :
Size        :
-
Title       :
Content     :
Assigned Person :
Size        :

DONE Line
************************
~ EMPTY ~
Enter Title                                    : 
Enter Content                                  :
Select Size -> XS(1), S(2), M(3), L(4), XL(5)  :
Select Person                                  : 
**Sizes should be stored as Enums. When displaying, they should be shown as XS. When entering, the user should enter 1.

**Team members should be defined in a pre-existing list. (There is no need to dynamically define them within the program.) When defining a card, the user should be prompted for the team member's ID. If the entered ID is not valid, the process can be canceled with the message "Invalid entries!"
(3) Delete Card from Board

First, you need to select the card you want to delete.
Please enter the card title:

The card that meets your criteria could not be found on the board. Please make a selection.
* To end the deletion: (1)
* To try again: (2)
** If there are multiple cards with the same name, both can be deleted.

(4) Move Card
First, you need to select the card you want to move.
Please enter the card title:
If the card is not found:

The card that meets your criteria could not be found on the board. Please make a selection.
* To end the process: (1)
* To try again: (2)
If the card is found:

Found Card Details:
**************************************
Title       :
Content     :
Assigned Person :
Size        :
Line        :

Please select the Line to move to:
(1) TODO
(2) IN PROGRESS
(3) DONE
** If a correct selection is made, the board is displayed using (1) List Boards. If the selection is incorrect, the process can be terminated with the message "You made an incorrect selection!"


