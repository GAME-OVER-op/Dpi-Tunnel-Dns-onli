# DPI Tunnel + Dns onli

**Версия:** 2.5 и 2.6 от 24.05.2024 и 04.06.2024  
**Разработчики:** nomoresat, Ggover  
**Статус:** Проект приостановлен на технические переработки. Ждите обновлений.  
**Русский интерфейс:** Да  
**Технические требования:** Android 11+, Magisk 19+

## Описание:
Модуль устанавливает приложение DPI Tunnel с повышенными правами доступа, что позволяет обходить замедление сервисов Google. Это ускоряет работу YouTube и Google Photos, улучшает доступ к сервисам ИИ и блокирует некоторую рекламу.

### Доступные версии модуля:
- **С DNS:** Версия модуля с встроенным DNS от Comss для улучшения сетевой конфиденциальности.
- **Без DNS:** Легкая версия модуля без встроенного DNS, для тех, кто предпочитает использовать свои собственные настройки DNS.
- **С DNS и прокси для локальной сети:** Версия модуля с DNS от Comss и локальным прокси-сервером для оптимизации работы в локальной сети.

## Установка и удаление:
- После установки и перезагрузки устройства, выполните еще одну перезагрузку для корректного применения DNS параметров.
- После удаления модуля и перезагрузки системы, телефон автоматически перезагрузится снова в течение минуты для очистки остаточных файлов.

## Инструкция по настройке:
1. Запустите приложение и предоставьте root-доступ.
2. Перейдите во вкладку 'Профили'.
3. Удалите все существующие профили и создайте новый, нажав кнопку "+".
4. Нажмите кнопку "Подобрать настройки".
5. Введите ссылку (например, `m.youtube.com`) и нажмите "ОК".
6. Появятся новые параметры для настройки.
7. Включите "Неверный SEQ" для поддельных пакетов.
8. Включите автоматический подбор TTL.
9. Включите опцию "Разбивать ClientHello по середине SNI".
10. Установите позицию для разбиения запроса на 6 или выше.
11. Сохраните настройки, нажав кнопку в правом нижнем углу.
12. Запустите YouTube и выберите любое видео — оно должно загрузиться без задержек.
13. Скажите замедлению YouTube — НЕТ!

## Дополнительная информация:
- Если после удаления модуля у вас возникли проблемы, введите следующую команду в терминале под root:
  ```bash
  settings put global http_proxy ""


  # DPI Tunnel + Dns onli

**Version:** 2.5 and 2.6 from 24.05.2024 and 04.06.2024  
**Developers:** nomoresat, Ggover  
**Status:** Project suspended for technical revisions. Stay tuned for updates.  
**Russian interface:** Yes  
**Technical requirements:** Android 11+, Magisk 19+

## Description:
This module installs the DPI Tunnel application with elevated privileges, allowing you to bypass Google service slowdowns. It enhances the performance of YouTube and Google Photos, improves access to AI services, and blocks some ads.

### Available Module Versions:
- **With DNS:** This version includes DNS settings provided by Comss to enhance network privacy.
- **Without DNS:** A lightweight version without integrated DNS, for users who prefer to use their own DNS settings.
- **With DNS and Local Network Proxy:** This version includes Comss DNS and a local network proxy for optimizing performance on a local network.

## Installation and Removal:
- After installation and rebooting the device, reboot the phone again to correctly apply DNS settings.
- After removing the module and rebooting the system, the phone will automatically reboot again within a minute to clear residual files.

## Setup Instructions:
1. Launch the application and grant root access.
2. Go to the 'Profiles' tab.
3. Delete all existing profiles and create a new one by clicking the "+" button.
4. Click the "Select settings" button.
5. Enter a URL (e.g., `m.youtube.com`) and click "OK".
6. New settings options will appear.
7. Enable "Incorrect SEQ" for fake packets.
8. Enable automatic TTL selection.
9. Enable the "Split ClientHello in the middle of SNI" option.
10. Set the request split position to 6 or higher.
11. Save the settings by clicking the button at the bottom right corner.
12. Launch YouTube and play any video — it should load without delays.
13. Say NO to YouTube slowdown!

## Additional information:
- If you encounter issues after uninstalling the module, enter the following command in the terminal under root:
  ```bash
  settings put global http_proxy ""
