# Kicad_Proects

****************************

Kicad and EasyEda Proects.

Проекты Kicad и Easyeda.

<img src="https://raw.githubusercontent.com/maximalisimus/Kicad_Library/main/images/Shadow-Projects-image.jpg"  height="400">

<a name="Oglavlenie"></a>

## Оглавление

1. [Библиотеки](#Libs)
2. [Настройки](#Config)
3. [About](#About)


## <a name="Libs">Библиотеки</a>

Библиотеки находятся по адресу: [Kicad-Libraries](https://github.com/maximalisimus/Kicad_Library.git)

Данные библиотеки специально сделаны для **Kicad**.

**3D Модели сохранены в нескольких форматах:**
* .stl
* .wrl
* .stp and .step

На сайте **EasyEda** преимущественно используются модели в формате **wrl**.

В **Kicad** можно использовать 3D модели 2 форматов: **stp** и **wrl**.

---

[К оглавлению](#Oglavlenie)

## <a name="Config">Настройки</a>

После запуска программы **Kicad**, откройте **меню** -> **Настройки** -> **Настройки путей** и добавте нижеуказанную строку.

**Linux**:

| Имя           | Путь                                          |
| --------------| ----------------------------------------------|
| KICAD_LIBRARY | /home/mikl/git_ssh/Kicad_Library/Shadow-Lib/  |

**Windows**:

| Имя           | Путь                               |
| --------------| -----------------------------------|
| KICAD_LIBRARY | D:\Temp\Kicad_Library\Shadow-Lib\  |

А далее, в **менеджере библиотек компонентов** и **менеджере библиотек посад.мест** добавьте в список глобальных библиотек для каждой библиотеки следующие строки.

Таблица **менеджера библиотек компонентов** - **Linux**:

| Использовать  | Уникальное имя   | Путь библиотеки                                      | Тип плагина | Параметры | Описание |
| --------------| -----------------| -----------------------------------------------------| ------------| ----------| ---------|
| ✓             | S-Trans-Coils    | ${KICAD_LIBRARY}/Shadow-Symbols/S-Trans-Coils.lib    | Legacy      |           |          |
| ✓             | S-Semiconductors | ${KICAD_LIBRARY}/Shadow-Symbols/S-Semiconductors.lib | Legacy      |           |          |
| ✓             | S-Resistance     | ${KICAD_LIBRARY}/Shadow-Symbols/S-Resistance.lib     | Legacy      |           |          |
| ✓             | S-Relay          | ${KICAD_LIBRARY}/Shadow-Symbols/S-Relay.lib          | Legacy      |           |          |
| ✓             | S-Modules        | ${KICAD_LIBRARY}/Shadow-Symbols/S-Modules.lib        | Legacy      |           |          |
| ✓             | S-Displays       | ${KICAD_LIBRARY}/Shadow-Symbols/S-Displays.lib       | Legacy      |           |          |
| ✓             | S-Connectors     | ${KICAD_LIBRARY}/Shadow-Symbols/S-Connectors.lib     | Legacy      |           |          |
| ✓             | S-Chips          | ${KICAD_LIBRARY}/Shadow-Symbols/S-Chips.lib          | Legacy      |           |          |
| ✓             | S-Capacitors     | ${KICAD_LIBRARY}/Shadow-Symbols/S-Capacitors.lib     | Legacy      |           |          |

Таблица **менеджера библиотек компонентов** - **Windows**:

| Использовать  | Уникальное имя   | Путь библиотеки                                      | Тип плагина | Параметры | Описание |
| --------------| -----------------| -----------------------------------------------------| ------------| ----------| ---------|
| ✓             | S-Trans-Coils    | ${KICAD_LIBRARY}\Shadow-Symbols\S-Trans-Coils.lib    | Legacy      |           |          |
| ✓             | S-Semiconductors | ${KICAD_LIBRARY}\Shadow-Symbols\S-Semiconductors.lib | Legacy      |           |          |
| ✓             | S-Resistance     | ${KICAD_LIBRARY}\Shadow-Symbols\S-Resistance.lib     | Legacy      |           |          |
| ✓             | S-Relay          | ${KICAD_LIBRARY}\Shadow-Symbols\S-Relay.lib          | Legacy      |           |          |
| ✓             | S-Modules        | ${KICAD_LIBRARY}\Shadow-Symbols\S-Modules.lib        | Legacy      |           |          |
| ✓             | S-Displays       | ${KICAD_LIBRARY}\Shadow-Symbols\S-Displays.lib       | Legacy      |           |          |
| ✓             | S-Connectors     | ${KICAD_LIBRARY}\Shadow-Symbols\S-Connectors.lib     | Legacy      |           |          |
| ✓             | S-Chips          | ${KICAD_LIBRARY}\Shadow-Symbols\S-Chips.lib          | Legacy      |           |          |
| ✓             | S-Capacitors     | ${KICAD_LIBRARY}\Shadow-Symbols\S-Capacitors.lib     | Legacy      |           |          |

Глобальная таблица **Symbols** в **Linux** находится в файле: **"$HOME/.config/.config/kicad/sym-lib-table"**.

Глобальная таблица **Symbols** в **Windows** находится в файле: **"C:\Users\USERS\AppData\Roaming\kicad\sym-lib-table"** или **"%AppData%\kicad\sym-lib-table"**.

Можно просто скопировать код ниже между 1 и последней строкой и вставить в данную таблицу вручную, чтобы не мучаться с долгой вставкой каждой библиотеки выше.

Редактирование данных файлов можно осуществить с помощью утилиты **Notepad++**. Все пути соответственно поправьте. 

**sym-lib-table - Linux**:
```
(sym_lib_table
  (lib (name S-Trans-Coils)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Trans-Coils.lib)(options "")(descr ""))
  (lib (name S-Semiconductors)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Semiconductors.lib)(options "")(descr ""))
  (lib (name S-Resistance)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Resistance.lib)(options "")(descr ""))
  (lib (name S-Relay)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Relay.lib)(options "")(descr ""))
  (lib (name S-Modules)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Modules.lib)(options "")(descr ""))
  (lib (name S-Displays)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Displays.lib)(options "")(descr ""))
  (lib (name S-Connectors)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Connectors.lib)(options "")(descr ""))
  (lib (name S-Chips)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Chips.lib)(options "")(descr ""))
  (lib (name S-Capacitors)(type Legacy)(uri ${KICAD_LIBRARY}/Shadow-Symbols/S-Capacitors.lib)(options "")(descr ""))
)
```

**sym-lib-table - Windows**:

```
(sym_lib_table
  (lib (name S-Trans-Coils)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Trans-Coils.lib)(options "")(descr ""))
  (lib (name S-Semiconductors)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Semiconductors.lib)(options "")(descr ""))
  (lib (name S-Resistance)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Resistance.lib)(options "")(descr ""))
  (lib (name S-Relay)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Relay.lib)(options "")(descr ""))
  (lib (name S-Modules)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Modules.lib)(options "")(descr ""))
  (lib (name S-Displays)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Displays.lib)(options "")(descr ""))
  (lib (name S-Connectors)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Connectors.lib)(options "")(descr ""))
  (lib (name S-Chips)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Chips.lib)(options "")(descr ""))
  (lib (name S-Capacitors)(type Legacy)(uri ${KICAD_LIBRARY}\Shadow-Symbols\S-Capacitors.lib)(options "")(descr ""))
)
```

Таблица **менеджера библиотек посад.мест** - **Linux**:

| Использовать | Уникальное имя   | Путь библиотеки                                            | Тип плагина | Параметры | Описание |
| -------------| -----------------| -----------------------------------------------------------| ------------| ----------| ---------|
| ✓            | S-Trans-Coils    | ${KICAD_LIBRARY}/Shadow-Footprints/S-Trans-Coils.pretty    | KiCad       |           |          |
| ✓            | S-Semiconductors | ${KICAD_LIBRARY}/Shadow-Footprints/S-Semiconductors.pretty | KiCad       |           |          |
| ✓            | S-Resistance     | ${KICAD_LIBRARY}/Shadow-Footprints/S-Resistance.pretty     | KiCad       |           |          |
| ✓            | S-Relay          | ${KICAD_LIBRARY}/Shadow-Footprints/S-Relay.pretty          | KiCad       |           |          |
| ✓            | S-Modules        | ${KICAD_LIBRARY}/Shadow-Footprints/S-Modules.pretty        | KiCad       |           |          |
| ✓            | S-Displays       | ${KICAD_LIBRARY}/Shadow-Footprints/S-Displays.pretty       | KiCad       |           |          |
| ✓            | S-Connectors     | ${KICAD_LIBRARY}/Shadow-Footprints/S-Connectors.pretty     | KiCad       |           |          |
| ✓            | S-Chips          | ${KICAD_LIBRARY}/Shadow-Footprints/S-Chips.pretty          | KiCad       |           |          |
| ✓            | S-Capacitors     | ${KICAD_LIBRARY}/Shadow-Footprints/S-Capacitors.pretty     | KiCad       |           |          |

Таблица **менеджера библиотек посад.мест** - **Windows**:

| Использовать | Уникальное имя   | Путь библиотеки                                            | Тип плагина | Параметры | Описание |
| -------------| -----------------| -----------------------------------------------------------| ------------| ----------| ---------|
| ✓            | S-Trans-Coils    | ${KICAD_LIBRARY}\Shadow-Footprints\S-Trans-Coils.pretty    | KiCad       |           |          |
| ✓            | S-Semiconductors | ${KICAD_LIBRARY}\Shadow-Footprints\S-Semiconductors.pretty | KiCad       |           |          |
| ✓            | S-Resistance     | ${KICAD_LIBRARY}\Shadow-Footprints\S-Resistance.pretty     | KiCad       |           |          |
| ✓            | S-Relay          | ${KICAD_LIBRARY}\Shadow-Footprints\S-Relay.pretty          | KiCad       |           |          |
| ✓            | S-Modules        | ${KICAD_LIBRARY}\Shadow-Footprints\S-Modules.pretty        | KiCad       |           |          |
| ✓            | S-Displays       | ${KICAD_LIBRARY}\Shadow-Footprints\S-Displays.pretty       | KiCad       |           |          |
| ✓            | S-Connectors     | ${KICAD_LIBRARY}\Shadow-Footprints\S-Connectors.pretty     | KiCad       |           |          |
| ✓            | S-Chips          | ${KICAD_LIBRARY}\Shadow-Footprints\S-Chips.pretty          | KiCad       |           |          |
| ✓            | S-Capacitors     | ${KICAD_LIBRARY}\Shadow-Footprints\S-Capacitors.pretty     | KiCad       |           |          |

Глобальная таблица **Footprints** в **Linux** находится в файле: **"$HOME/.config/.config/kicad/fp-lib-table"**.

Глобальная таблица **Footprints** в **Windows** находится в файле: **"C:\Users\USERS\AppData\Roaming\kicad\fp-lib-table"** или **"%AppData%\kicad\fp-lib-table"**.

Можно просто скопировать код ниже между 1 и последней строкой и вставить в данную таблицу вручную, чтобы не мучаться с долгой вставкой каждой библиотеки выше.

Редактирование данных файлов можно осуществить с помощью утилиты **Notepad++**. Все пути соответственно поправьте.

**fp-lib-table - Linux**:

```
(fp_lib_table
  (lib (name S-Trans-Coils)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Trans-Coils.pretty)(options "")(descr ""))
  (lib (name S-Semiconductors)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Semiconductors.pretty)(options "")(descr ""))
  (lib (name S-Resistance)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Resistance.pretty)(options "")(descr ""))
  (lib (name S-Connectors)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Connectors.pretty)(options "")(descr ""))
  (lib (name S-Capacitors)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Capacitors.pretty)(options "")(descr ""))
  (lib (name S-Modules)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Modules.pretty)(options "")(descr ""))
  (lib (name S-Chips)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Chips.pretty)(options "")(descr ""))
  (lib (name S-Relay)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Relay.pretty)(options "")(descr ""))
  (lib (name S-Displays)(type KiCad)(uri ${KICAD_LIBRARY}/Shadow-Footprints/S-Displays.pretty)(options "")(descr ""))
)
```

**fp-lib-table - Windows**:

```
(fp_lib_table
  (lib (name S-Trans-Coils)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Trans-Coils.pretty)(options "")(descr ""))
  (lib (name S-Semiconductors)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Semiconductors.pretty)(options "")(descr ""))
  (lib (name S-Resistance)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Resistance.pretty)(options "")(descr ""))
  (lib (name S-Connectors)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Connectors.pretty)(options "")(descr ""))
  (lib (name S-Capacitors)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Capacitors.pretty)(options "")(descr ""))
  (lib (name S-Modules)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Modules.pretty)(options "")(descr ""))
  (lib (name S-Chips)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Chips.pretty)(options "")(descr ""))
  (lib (name S-Relay)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Relay.pretty)(options "")(descr ""))
  (lib (name S-Displays)(type KiCad)(uri ${KICAD_LIBRARY}\Shadow-Footprints\S-Displays.pretty)(options "")(descr ""))
)
```

---

[К оглавлению](#Oglavlenie)

## <a name="About">About</a>

Автор проектов: [maximalisimus](https://github.com/maximalisimus).
