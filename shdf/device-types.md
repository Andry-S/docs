# Типы (коды) устройств ШДФ

## Ссылки

- [Документация ШДФ](/shdf/)
  - [Карта памяти заданных типов устройств ШДФ](/shdf/devices-map.md)
  - [**Типы (коды) устройств ШДФ**](/shdf/device-types.md)
  - [Карты памяти устройств ШДФ:](/shdf/maps/)
    - [`[0002] Дискретный вход`](/shdf/maps/di%20[0002].md)
    - [`[8003] Мастер дискретных выходов`](/shdf/maps/mdo%20[8003].md)

## Коды устройств

_Таблица 1. Таблица кодов устройств_

<table summary="Таблица кодов устройств" border="1">
    <tbody valign="center" align="center">
        <tr>
            <td><strong>Код (шестн.)</strong></td>
            <td align="left"><strong>Наименование</strong></td>
            <td><strong>MROM</strong></td>
            <td><strong>EEPROM</strong></td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Простые устройства (входа выхода и т.п.)</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x0001</strong></code></td>
            <td align="left"><a href="/shdf/maps/empty%20[0001].md">Пустое устройство (тест)</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x8001</strong></code></td>
            <td align="left"><a href="/shdf/maps/mezo%20master%20[80001].md">Мастер состояния мезонинов</a></td>
            <td>28</td>
            <td>48</td>
        </tr>
        <tr>
            <td><code><strong>0x0002</strong></code></td>
            <td align="left"><a href="/shdf/maps/di%20[0002].md">Дискретный вход</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x8002</strong></code></td>
            <td align="left"><a href="/shdf/maps/mdi%20[8002].md">Мастер дискретных входов</a></td>
            <td>N / 8 + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x0003</strong></code></td>
            <td align="left"><a href="/shdf/maps/do%20[0003].md">Дискретный выход</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x8003</strong></code></td>
            <td align="left"><a href="/shdf/maps/mdo%20[8003].md">Мастер дискретных выходов</a></td>
            <td>N / 8 + 4 + N</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x0004</strong></code></td>
            <td align="left"><a href="/shdf/maps/ai%20[0004].md">Аналоговый вход</a></td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>0x8004</strong></code></td>
            <td align="left"><a href="maps/mai%20[8004].md">Мастер аналоговых входов</a></td>
            <td>12 * N + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x0041</strong></code></td>
            <td align="left"><a href="/shdf/maps/ao%20[0041].md">Аналоговый выход</a></td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>0x0006</strong></code></td>
            <td align="left"><a href="/shdf/maps/pu%20[0006].md">Мезонин питания СР6761</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x6921</strong></code></td>
            <td align="left"><a href="/shdf/maps/rc%20[6921].md">Мезонин подключения пульта СР6921</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Составные устройства (в составе ссылки на простые либо составные устройства)</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x0135</strong></code></td>
            <td align="left">Регулятор 6835</td>
            <td>64</td>
            <td>92</td>
        </tr>
        <tr>
            <td><code><strong>0x0136</strong></code></td>
            <td align="left">Регулятор 6836</td>
            <td>64</td>
            <td>160</td>
        </tr>
        <tr>
            <td><code><strong>0x0247</strong></code></td>
            <td align="left">Задвижка 6847</td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6851</strong></code></td>
            <td align="left">Насос 6851</td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6852</strong></code></td>
            <td align="left">Насосная станция 6852</td>
            <td>52</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6854</strong></code></td>
            <td align="left">Насосная станция 6854</td>
            <td>64</td>
            <td>32</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Логика и интерфейсы</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x7001</strong></code></td>
            <td align="left">Простая логика тип 1 (дискретная)</td>
            <td>4</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>0x7002</strong></code></td>
            <td align="left">Простая логика тип 2 (вещественная, пороги)</td>
            <td>8</td>
            <td>40</td>
        </tr>
        <tr>
            <td><code><strong>0x7011</strong></code></td>
            <td align="left">Передача, синхронизация двух битовых переменных в MROM</td>
            <td>4</td>
            <td>16</td>
        </tr>
        <tr>
            <td><code><strong>0x7020</strong></code></td>
            <td align="left">Передача, синхронизация двух вещественных переменных в MROM</td>
            <td>16</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x6881</strong></code></td>
            <td align="left">Шлюз 6881 - RS485</td>
            <td>8</td>
            <td>32</td>
        </tr>
        <tr>
            <td><code><strong>0x6891</strong></code></td>
            <td align="left">Обработчик данных шлюза (преобразование пакета в список переменных)</td>
            <td>136</td>
            <td>72</td>
        </tr>
        <tr>
            <td><code><strong>0x6880</strong></code></td>
            <td align="left">Ethernet ретранслятор</td>
            <td>8</td>
            <td>20</td>
        </tr>
    </tbody>
</table>
