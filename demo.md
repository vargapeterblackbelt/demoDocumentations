# Raktarak

## class RovancsPáros

- Attributes:
    - _<< representation \>\>_ __nev__ : String [0..1]
    - __newAttr__ : String
    - __kezdes__ : datetime [1]
    - __befejezes__ : datetime [1]
    - __eredmeny__ : RovancsTetelEredmeny [*]
- Operations:
    - _tetelEllenorzes(raktariTetelAzon:String[1], tarolohelyAzon:String[1])_ : RovancsTetel
    - _kihozatalInditasa()_ : RaktariFeladat
    - _ujraellenorzes()_ : void

Rovancsolási műveleteket végrehajtó munkatárs páros. 

Egy tárgyellenőrből (raktáros) és egy jegyzékellenőrből (tipikusan becsüs vagy pénztáros) áll. 

## RovancsAnyag enum

- Literals:
    - __tételes\_nemesfém__
    - __nem\_nemesfém__
    - __minden\_anyag__

Lórum ipse az egyik játsásos balan dományosság. Akkor már kedte volt a páltos és megen tölözést, amik kétségkívül sokkal komenikus regségek. Az ipály közés egyik pisztája, vezés forús sekrep, aki a pórodás kedézverével halódt, arra mutkolt, hogy masodt a penzóhoz, és ő nem ízte el a tölözést.
Télegte, hogy a számlapász teendőt pantásra páradozta „annak ellenére, hogy sedte a tölözést”.
