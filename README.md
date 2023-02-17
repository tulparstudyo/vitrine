# vitrine
opencart 4x tem yazım kuralları

1. oc_extension_path dosyasında temanın kayıtlı olması gerekir modül yüklenirken otomatik oluşması için modül dosyasında 

  extension/****/admin/controller/theme/****.php  olmalıdır
  
  Dil dosyasını extension/vitrine/admin/language/en-gb/theme/****.php koyun ve
  
  $_['heading_title'] = '**** Template'; 
  
  Not: eklenti dosyasının kurulabilmesi için içide install.json zorunludur.
