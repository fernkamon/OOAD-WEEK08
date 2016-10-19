# OOAD-WEEK08

## ส่งการบ้าน เรื่อง Use Case Diagram 5 ภาพ

* ภาพที่ 1 บัญชีธนาคาร

```
@startuml

:Bank Employee: -> (Start)
:Bank Employee:  --> (Bank Account) : Manage data accoording\nto customer\nrequiements

:Customer: ---> (Bank Account) : Deposit\nWithdraw\ntransfer money

@enduml
```

![](http://www.plantuml.com/plantuml/img/ROyx3i8m44Hxds9BKd015oZyIYeAcZGhUmaMyMvYhuLoUsn41-NCazve-goOjCJ967j0Vi8vpfEiH1QsEzXS6-r-KMEVRk-S5DOEB5oGSIJmg0XOQqa-y0W3gu0hMILIgYdHKW95Oirry_W5pVbFUg9PSj21Rq4VFk6hwX9olbTN5ARLc9xOrmDl)

* ภาพที่ 2 การใช้ตู้ ATM

```
@startuml
title <b> User <b> ATM
:user: -left-> (Deposit) 
:user: -right-> (Withdrawal) 
:user: -up-> (Transfer money)
:user: -down-> (Check Balance)
@enduml
```

![](http://www.plantuml.com/plantuml/img/JSux3eCm40JGtgVOCYwu08eG-RJfGAaNlCHM5Xkj5w7Sdaz3oj4RZQREYgBpo4Q3CW6qcGIkNNLhNgOyKWa5qw151PSdJIa7jN2IX8y_x1tKEy45-P_dQRT6CEPX6nvJf9yzsQKbxeM7f_uBTsICFLbJKtJRfnK0)

* ภาพที่ 3 การใช้บริการโรงเเรม

```
@startuml
left to right direction
skinparam packageStyle rect
actor customer
actor clerk
rectangle Hotel {
  customer -- (payment)
  customer -- (checkout)
  customer -- (stay)
  customer -- (checkin)
  (checkin) .> (stay) 
  (stay) .> (checkout) 
  (checkout) .> (payment)
  (checkin) -- clerk
  (payment) -- clerk
}
@enduml
```

![](http://www.plantuml.com/plantuml/img/RP3B3e8m44Nt_Ogxr0L-Wc7ftY-Ob16QliWmB8ZntuL6G8FBdZEzywW79T4n1XFueT0CSMsdQ9omLPUJ6RnBFGb5z6GzjNpNAJ2mU4DMiy2EW-R8iZu3YpUBfzJEfRUi7F0qs0fHLJZPZgtFevx_2fSEV1vrEi2UfiYfXEo9k5n_JVbQw7VNhLCnQ_nEgyygsCCszZ8rfsO-t1i0)

* ภาพที่ 4 การตรวจสอบสิทธิ์การใช้บัตรเครดิต

```
@startuml
left to right direction
skinparam packageStyle rect
actor customer
actor :Retail Institution:
actor :Soonsoring Financial InInstitution:
rectangle  {
  customer -- (Perform Card Transaction)
  customer -- (Process Customer Bill)
  customer -- (Manage Customer Account)
  (Perform Card Transaction) -- :Retail Institution: 
  (Recocile Transactions) -- :Retail Institution: 
  (Process Customer Bill) -- :Retail Institution:
  (Process Customer Bill) -- :Soonsoring Financial InInstitution:
  (Manage Customer Account) -- :Soonsoring Financial InInstitution:
}
@enduml
```

![](http://www.plantuml.com/plantuml/img/hPBDJWCn38JlUGeVwQ4liAVIbP0u8A5knTrAtCLgObUEzr0XtfqiY1zH5d7WcfblD1vbKntDfvB3dZqJz4Q97Ngq10-OEQ6p2WpdwbH2feE3AnYFZmw9ZU8iXtfaEQ5XWHF68uuq-Bc5pNB0w6eGf-fQo4At8qVES2lLsQSPxq8tg4fLOndXXWKbCdwpp5aeOqk5fm0VUR1UmzKzsK6jlBNU6qh5rrwh2wDff5gXVt_SSiuNhZkKTiAdwJf6dSHdtwBMm3yS0KiL_W7_QTS6x2Xgv3RRbrtgRy3Yc4lCSzYGfFQ5NW00)

* ภาพที่ 5 การลงทะเบียนเรียน

```
@startuml
title  credit Card Validation System
left to right direction
skinparam packageStyle rect
actor authoritiesr
actor Student
rectangle  {
  authoritiesr -- (Registration for new student) : <<usser>>
  authoritiesr -- (Current Student Registration) : <<usser>>
  (Registration for new student) --> (evidence collection) : <<usser>>
  (Current Student Registration) --> (evidence collection) : <<usser>>
  (Registration for new student) --> (Payment Fees) : <<usser>>
  (Current Student Registration) --> (Payment Fees) : <<usser>>
  (Payment Fees) ..> (Except) : <<extends>>
  (Payment Fees) ..> (No Payment Fees) : <<extends>>
  (evidence collection) ..> (The evidence is not available) : <<extends>>
  (Payment Fees) -- Student
}
@enduml
```

![](http://www.plantuml.com/plantuml/img/dLBDJiCm3BxdANmSX-u1q5HDck2844NSJUgrrjAaSjon2l7kf7H3b8rjufXylt6yZ8gYNUECiZe2i48bAwnGIdX1noKg1mz57vKQusYje064grgXP24xm2PksBSes42BTeCL5Tedjm4sQ3K8OATr45QcAFkhGhkIl9g1XRuQqjyDJ9YGPJ1xeegZobXadOIUtY2EuXkuXSMYYv4apq-9Lvr8uXt2uAVPR_65f2pBOKPRJYTBO8Dpu-kFRCvdNcrpHPj7x9iXuPue_gV6MVqKdCyJ_svdgTqFdNPAlen_SXy27DjFH2U7yALzhWc-KOxWWm9kaHs-EheOd_xzi5iVPfbOQRy_0G00)

### Use Case Diagram (ภาษาไทย)
* บรรยายเรื่อง UML โดย อ.ปานใจ  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/0eq2FGEQul8/0.jpg)](http://www.youtube.com/watch?v=0eq2FGEQul8 "บรรยายเรื่อง UML โดย อ.ปานใจ  " target="_blank") 

* เรียนการออกแบบโปรแกรมด้วย UML กับโปรเอิ๊ก ตอนที่ 1 การเขียน Requirement Card และ Use case   

[![IMAGE ALT TEXT](http://img.youtube.com/vi/u9sNT6x0Mlo/0.jpg)](http://www.youtube.com/watch?v=u9sNT6x0Mlo "เรียนการออกแบบโปรแกรมด้วย UML กับโปรเอิ๊ก ตอนที่ 1 การเขียน Requirement Card และ Use case " target="_blank") 

* How to draw a UML Use Case Diagram

[![IMAGE ALT TEXT](http://img.youtube.com/vi/UzprPX82Nac/0.jpg)](http://www.youtube.com/watch?v=UzprPX82Nac "How to draw a UML Use Case Diagram" target="_blank") 

## Use Case Diagram Tutorial (VTC)

* 3.01_Use Case Basics  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/tLJXJLfLCCM/0.jpg)](http://www.youtube.com/watch?v=tLJXJLfLCCM " 3.01_Use Case Basics " target="_blank") 

* 3.02_Modeling Use Case Elements  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/_JCsqdNf8bA/0.jpg)](http://www.youtube.com/watch?v=_JCsqdNf8bA " 3.02_Modeling Use Case Elements " target="_blank") 
 
* 3.03_A Use Case Diagram for an ATM  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/SmcBTsPsbIY/0.jpg)](http://www.youtube.com/watch?v=SmcBTsPsbIY " 3.03_A Use Case Diagram for an ATM" target="_blank") 

 

* 3.04_The ''include'' Dependency  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/q7O2EAZ_s7M/0.jpg)](http://www.youtube.com/watch?v=q7O2EAZ_s7M " 3.04_The ''include'' Dependency " target="_blank") 

 

* 3.05_The ''extend'' Dependency  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/bL_Bl_Xl7wQ/0.jpg)](http://www.youtube.com/watch?v=bL_Bl_Xl7wQ " 3.05_The ''extend'' Dependency" target="_blank") 

 
* 3.06_Generalization  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/x5LkaZlLT28/0.jpg)](http://www.youtube.com/watch?v=x5LkaZlLT28 " 3.06_Generalization" target="_blank") 

 
* 3.07_Putting It All Together  

[![IMAGE ALT TEXT](http://img.youtube.com/vi/gYmOzpU7DDI/0.jpg)](http://www.youtube.com/watch?v=gYmOzpU7DDI " 3.07_Putting It All Together" target="_blank") 
 
