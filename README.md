<h1 align="center">EnderLauncher</h1>

<img src="app_pojavlauncher/src/main/assets/pojavlauncher.png" align="left" width="130" height="150" alt="EnderLauncher logo">

[![Android CI](https://github.com/deckt1me/EnderLauncher/workflows/Android%20CI/badge.svg)](https://github.com/deckt1me/EnderLauncher/actions)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/deckt1me/EnderLauncher)](https://github.com/deckt1me/EnderLauncher/actions)
[![Telegram](https://img.shields.io/badge/Telegram-Ender__Launcher-blue?logo=telegram)](https://t.me/Ender_Launcher)

EnderLauncher — лаунчер для запуска Minecraft: Java Edition на Android, основанный на [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher).

## Содержание

* [Введение](#введение)
* [Скачать](#скачать)
* [Сборка](#сборка)
* [Статус](#статус)
* [Известные проблемы](#известные-проблемы)
* [Поддержка](#поддержка)
* [Лицензия](#лицензия)
* [Credits](#credits)

## Введение

* EnderLauncher — лаунчер Minecraft: Java Edition для Android, основан на [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher)
* Поддерживает почти все версии Minecraft от rd-132211 до последних снапшотов
* Поддерживается установка модов через Forge и Fabric
* Оптимизирован для работы на Android-устройствах

## Скачать

1. **GitHub Actions:** Скачать APK из [автоматических сборок](https://github.com/deckt1me/EnderLauncher/actions)
2. **Сборка из исходников:** Следуй инструкции ниже

## Сборка

### Быстрая сборка

```bash
git clone https://github.com/deckt1me/EnderLauncher.git
cd EnderLauncher
./gradlew :app_pojavlauncher:assembleDebug
```

APK будет в папке `app_pojavlauncher/build/outputs/apk/debug/`.

### Подробная сборка

1. **JRE:** Скачай `jre8-pojav` из [CI сборок](https://github.com/PojavLauncherTeam/android-openjdk-build-multiarch/actions)
2. **Список языков:**
   ```bash
   chmod +x scripts/languagelist_updater.sh
   bash scripts/languagelist_updater.sh
   ```
3. **Сборка GLFW stub:** `./gradlew :jre_lwjgl3glfw:build`
4. **Сборка лаунчера:** `./gradlew :app_pojavlauncher:assembleDebug`

## Статус

* [x] OpenJDK 8: ARM32, ARM64, x86, x86_64
* [x] OpenJDK 17: ARM32, ARM64, x86, x86_64
* [x] OpenJDK 21: ARM32, ARM64, x86, x86_64
* [x] Установщик модов (headless)
* [x] Установщик модов с GUI
* [x] OpenGL в среде OpenJDK
* [x] OpenAL (работает на большинстве устройств)
* [x] Поддержка Minecraft 1.12.2 и ниже
* [x] Поддержка Minecraft 1.13 и выше
* [x] Поддержка Minecraft 1.17 и выше
* [x] Масштабирование игрового экрана
* [x] Полностью переписанная система управления
* [ ] Ещё в разработке!

## Известные проблемы

Список известных проблем в [issue tracker](https://github.com/deckt1me/EnderLauncher/issues).

## Поддержка

По всем вопросам — Telegram канал: [t.me/Ender_Launcher](https://t.me/Ender_Launcher)

## Лицензия

EnderLauncher лицензирован под [GNU LGPLv3](LICENSE).

Основан на [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher) — [GNU LGPLv3](https://github.com/PojavLauncherTeam/PojavLauncher/blob/v3_openjdk/LICENSE).

## Credits

* [PojavLauncherTeam](https://github.com/PojavLauncherTeam/PojavLauncher) — основа лаунчера
* [Boardwalk](https://github.com/zhuowei/Boardwalk) — JVM Launcher
* [GL4ES](https://github.com/PojavLauncherTeam/gl4es) — MIT License
* [OpenJDK](https://github.com/PojavLauncherTeam/openjdk-multiarch-jdk8u) — GNU GPLv2
* [LWJGL3](https://github.com/PojavLauncherTeam/lwjgl3) — BSD-3 License
* [Mesa 3D](https://gitlab.freedesktop.org/mesa/mesa) — MIT License
* [bhook](https://github.com/bytedance/bhook) — MIT License
* [MCHeads](https://mc-heads.net) — аватары Minecraft
