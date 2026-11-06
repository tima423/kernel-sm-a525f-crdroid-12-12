# SM-A525F Kernel for crDroid 12.12

Русская версия — ниже.

## English

### Project status

This project is intended for the Samsung Galaxy A52 **SM-A525F** running
**crDroid 12.12**. Compatibility with a particular ROM build has not yet been
verified.

**The files currently provided are incomplete and are not a flashable release.**
The kernel Makefile identifies the source as Linux 4.14.357, but the supplied
tree has no files in `arch/arm64`, `drivers`, or `techpack`; it also contains no
SM-A525F defconfig, build script, or ready-to-flash image. The separate
`KernelSU-Next` directory is empty. Do not try to build or flash this source
drop as-is.

### Compatibility

- Device: **Samsung Galaxy A52 SM-A525F only**, unless a release explicitly
  lists other supported models.
- ROM: **crDroid 12.12** only when a release explicitly names the exact ROM
  build and required firmware.
- A matching Android version or ROM name alone does not guarantee kernel
  compatibility. Check the release notes before installing.

### Installation (for a future, explicitly released flashable package)

1. Read the release notes and verify the exact device model, ROM build, and
   firmware requirements.
2. Make a full recovery backup, including the boot-related partitions required
   by your device and recovery. Keep a copy of your current boot image or ROM
   so you can restore it.
3. Use only the package and installation method specified by that release.
   Do not flash a raw kernel image or use Odin/Fastboot unless the release
   maintainer explicitly instructs you to.
4. Reboot to recovery, flash the package as instructed, then reboot to Android.
5. If the device does not boot or important features stop working, return to
   recovery and restore your backup or the original boot image.

There is no flashable package in the source files currently provided.

### Building

Building is not possible from the current incomplete files. A buildable release
needs the complete device kernel source, the correct SM-A525F configuration,
the required compiler/toolchain, and tested build and packaging instructions.
Those items must be supplied and verified by the maintainer; generic kernel
commands are not a substitute for the device-specific configuration.

### Disclaimer

Kernel flashing can cause data loss or leave the device unable to boot. You are
responsible for checking compatibility and keeping a working backup. This
project is provided without a guarantee of functionality or support.

---

## Русский

### Статус проекта

Проект предназначен для Samsung Galaxy A52 **SM-A525F** с прошивкой
**crDroid 12.12**. Совместимость с конкретной сборкой прошивки пока не
проверена.

**Предоставленные сейчас файлы неполные и не являются готовой прошивкой для
установки.** По Makefile версия исходников — Linux 4.14.357, однако каталоги
`arch/arm64`, `drivers` и `techpack` в переданном дереве пусты. Также отсутствуют
конфигурация defconfig для SM-A525F, скрипт сборки и готовый образ для установки.
Отдельная папка `KernelSU-Next` тоже пустая. Не пытайтесь собирать или прошивать
эти файлы в текущем виде.

### Совместимость

- Устройство: только **Samsung Galaxy A52 SM-A525F**, если в релизе явно не
  указаны другие поддерживаемые модели.
- Прошивка: **crDroid 12.12**, только если в релизе указаны точная сборка ROM и
  необходимые версии firmware.
- Совпадение версии Android или названия ROM само по себе не гарантирует
  совместимость ядра. Перед установкой проверьте описание конкретного релиза.

### Установка (для будущего готового архива, явно опубликованного для прошивки)

1. Прочитайте описание релиза и проверьте точную модель устройства, сборку ROM и
   требования к firmware.
2. Создайте полную резервную копию через recovery, включая необходимые для
   устройства и recovery разделы, связанные с загрузкой. Сохраните копию
   исходного boot-образа или прошивки для восстановления.
3. Используйте только архив и способ установки, указанные в описании релиза.
   Не прошивайте отдельный raw-образ ядра и не используйте Odin/Fastboot, если
   автор релиза прямо этого не рекомендует.
4. Перезагрузитесь в recovery, установите архив по инструкции релиза и
   перезагрузите устройство в Android.
5. Если устройство не загружается или перестали работать важные функции,
   вернитесь в recovery и восстановите резервную копию или исходный boot-образ.

В предоставленных исходниках сейчас нет готового архива для прошивки.

### Сборка

Собрать ядро из текущего набора неполных файлов нельзя. Для готовой сборки нужны
полные исходники ядра устройства, правильная конфигурация SM-A525F, необходимый
компилятор/toolchain, а также проверенные инструкции по сборке и упаковке.
Эти материалы должен предоставить и проверить автор проекта; универсальные
команды сборки ядра не заменяют конфигурацию для конкретного устройства.

### Отказ от ответственности

Прошивка ядра может привести к потере данных или невозможности загрузить
устройство. Проверка совместимости и наличие рабочей резервной копии —
ответственность пользователя. Проект предоставляется без гарантии
работоспособности и поддержки.
