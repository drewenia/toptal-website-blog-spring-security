# Spring Authentication

- Authentication, kullanıcının sağladığı kimlik bilgilerini doğrulayarak kullanıcının kimliğini doğrulama sürecidir. Bir
  web sitesine giriş yaparken kullanıcı adı ve parola girmek gibi yaygın bir örnek verilebilir. Bunu, "Who are you?"
  sorusuna verilen bir yanıt olarak düşünebilirsiniz.

- Authorization, kullanıcının başarılı bir şekilde authenticate oldugu varsayımıyla belirli bir eylemi gerçekleştirmek
  veya belirli verileri okumak için uygun izne sahip olup olmadığını belirleme sürecidir. Bunu, "Bir kullanıcı bunu
  yapabilir/mi?" sorusuna verilen bir yanıt olarak düşünebilirsiniz.

- Principle, authenticated olan şu anki kullanıcıyı ifade eder. Bu terim, kimlik doğrulama işlemi başarılı olduğunda,
  kullanıcının temsil ettiği varlığı temsil etmek için kullanılır.

- Granted authority - Authenticated olan kullanıcının sahip olduğu permission'i ifade eder. Bir kullanıcının belirli
  eylemleri gerçekleştirmek veya belirli kaynaklara erişmek için yetkisi olabilir. Örneğin, bir kullanıcının "
  ROLE_ADMIN" veya "ROLE_USER" gibi rol veya yetkilendirme etiketlerine sahip olması, verilen yetkilere örnek olarak
  gösterilebilir.

Projeye spring security eklendiginde diger dependency'lerden farklı olarak anında tepki verir ve projenin tüm endpoint'
lerini korunaklı hale getirir. Proje ayağa kalktığında console da random bir şifre belirir. Herhangi bir endpoint'e
gitmeye çalıştığımız da otomatik olarak login page gelir. Default username olarak "user" password olarak da console da
bulunan generated password kullanılır