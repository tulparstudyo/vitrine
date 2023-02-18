# vitrine
opencart 4x tem yazım kuralları

1. oc_extension_path dosyasında temanın kayıtlı olması gerekir modül yüklenirken otomatik oluşması için modül dosyasında 

  extension/****/admin/controller/theme/****.php  olmalıdır
  
  Dil dosyasını extension/vitrine/admin/language/en-gb/theme/****.php koyun ve
  
  $_['heading_title'] = '**** Template'; 
  
  Not: eklenti dosyasının kurulabilmesi için içide install.json zorunludur.
  
2. system\config\catalog.php içinde $_['action_event']  değişkenine 'view/*/before' içine 999=>'extension/vitrine/theme/onepage|auto_loader' eklenerek theme dosyaları otomatik yüklenir.

3. Bir eklentiyi uninstal için öncellikle o eklenti ile oluşturulumuş modüllerin kaldırılması gerekir
