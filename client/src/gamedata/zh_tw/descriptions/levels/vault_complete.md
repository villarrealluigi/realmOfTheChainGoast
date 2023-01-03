一定請記住！將一個變數設成私用變數(private variable)，只能保證這個變數不被其他合約存取。設成私用的(private)狀態變數和本地變數，還是可以被公開的存取(publicly access)。

為了確保資料的隱私，資料在上鏈前需要被加密。在這種情況下，密鑰絕對不可以被送到鏈上，不然隨便一個有心人都可以輕易取得密鑰，這樣你的資料隱私就會蕩然無存。[zk-SNARKs](https://blog.ethereum.org/2016/12/05/zksnarks-in-a-nutshell/) 提供了一個可以驗證是否某使用者 A 有某一個秘密(secret)的方法，但是驗證的過程中又不需要揭露這個秘密。