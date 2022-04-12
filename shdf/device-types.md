# Типы (коды) устройств ШДФ

## Ссылки

- [Документация ШДФ](/shdf/)
  - [Карта памяти заданных типов устройств ШДФ](/shdf/devices-map.md)
  - [**Типы (коды) устройств ШДФ**](/shdf/device-types.md)
  - [Карты памяти устройств ШДФ:](/shdf/maps/)
    - [`[0001] Пустое устройство (тест)`](/shdf/maps/empty%20[0001].md)
    - [`[0002] Дискретный вход`](/shdf/maps/di%20[0002].md)
    - [`[0003] Дискретный выход`](/shdf/maps/do%20[0003].md)
    - [`[0004] Аналоговый вход`](/shdf/maps/ai%20[0004].md)
    - [`[0006] Мезонин питания СР6761`](/shdf/maps/pu%20[0006].md)
    - [`[0041] Аналоговый выход`](/shdf/maps/ao%20[0041].md)
    - [`[0135] Регулятор 6835`](/shdf/maps/reg%20[0135].md)
    - [`[0136] Регулятор 6836`](/shdf/maps/reg%20[0136].md)
    - [`[0247] Задвижка 6847`](/shdf/maps/valve%20[0247].md)
    - [`[6851] Насос 6851`](/shdf/maps/pump%20[6851].md)
    - [`[6852] Насосная станция 6852`](/shdf/maps/ps%20[6852].md)
    - [`[6853] Насос 6853`](/shdf/maps/pump%20[6853].md)
    - [`[6854] Насосная станция 6854`](/shdf/maps/ps%20[6854].md)
    - [`[6880] Ethernet ретранслятор`](/shdf/maps/ethernet%20[6880].md)
    - [`[6881] Шлюз 6881 - RS485`](/shdf/maps/gate%20[6881].md)
    - [`[6891] Обработчик данных шлюза (преобразование пакета в список переменных)`](/shdf/maps/gate%20[6891].md)
    - [`[6921] Мезонин подключения пульта СР6921`](/shdf/maps/rc%20[6921].md)
    - [`[7001] Простая логика тип 1 (дискретная)`](/shdf/maps/logic%20[7001].md)
    - [`[7002] Простая логика тип 2 (вещественная, пороги)`](/shdf/maps/logic%20[7002].md)
    - [`[7011] Передача, синхронизация двух битовых переменных в MROM`](/shdf/maps/sync%20[7011].md)
    - [`[7020] Передача, синхронизация двух вещественных переменных в MROM`](/shdf/maps/sync%20[7020].md)
    - [`[8001] Мастер состояния мезонинов`](/shdf/maps/mezo%20master%20[80001].md)
    - [`[8002] Мастер дискретных входов`](/shdf/maps/mdi%20[8002].md)
    - [`[8003] Мастер дискретных выходов`](/shdf/maps/mdo%20[8003].md)
    - [`[8004] Мастер аналоговых входов`](/shdf/maps/mai%20[8004].md)

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
            <td colspan="4" align="left"><strong>Простые устройства (входы, выходы и т.п.)</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x0002</strong></code></td>
            <td align="left"><a href="/shdf/maps/di%20[0002].md">Дискретный вход</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x0003</strong></code></td>
            <td align="left"><a href="/shdf/maps/do%20[0003].md">Дискретный выход</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>0x0004</strong></code></td>
            <td align="left"><a href="/shdf/maps/ai%20[0004].md">Аналоговый вход</a></td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>0x0041</strong></code></td>
            <td align="left"><a href="/shdf/maps/ao%20[0041].md">Аналоговый выход</a></td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>??? 0x0006</strong></code></td>
            <td align="left"><a href="/shdf/maps/pu%20[0006].md">Мезонин питания СР6761</a></td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td><code><strong>??? 0x6921</strong></code></td>
            <td align="left"><a href="/shdf/maps/rc%20[6921].md">Мезонин подключения пульта СР6921</a></td>
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
            <td><code><strong>0x8002</strong></code></td>
            <td align="left"><a href="/shdf/maps/mdi%20[8002].md">Мастер дискретных входов</a></td>
            <td><i>N<sub>вх</sub></i> / 8 + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x8003</strong></code></td>
            <td align="left"><a href="/shdf/maps/mdo%20[8003].md">Мастер дискретных выходов</a></td>
            <td><i>N<sub>вых</sub></i> / 8 + 4 + N<sub>вых</sub></td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x8004</strong></code></td>
            <td align="left"><a href="maps/mai%20[8004].md">Мастер аналоговых входов</a></td>
            <td>12 * <i>N<sub>вх</sub></i> + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Составные устройства (в составе ссылки на простые либо составные устройства)</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x0135</strong></code></td>
            <td align="left"><a href="/shdf/maps/reg%20[0135].md">Регулятор СР6835</a></td>
            <td>64</td>
            <td>92</td>
        </tr>
        <tr>
            <td><code><strong>0x0136</strong></code></td>
            <td align="left"><a href="/shdf/maps/reg%20[0136].md">Регулятор СР6836</a></td>
            <td>64</td>
            <td>160</td>
        </tr>
        <tr>
            <td><code><strong>0x0247</strong></code></td>
            <td align="left"><a href="/shdf/maps/valve%20[0247].md">Задвижка СР6847</a></td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6851</strong></code></td>
            <td align="left"><a href="/shdf/maps/pump%20[6851].md">Насос 6851</a></td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6852</strong></code></td>
            <td align="left"><a href="/shdf/maps/ps%20[6852].md">Насосная станция 6852</a></td>
            <td>52</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6853</strong></code></td>
            <td align="left"><a href="/shdf/maps/pump%20[6853].md">Насос 6853</a></td>
            <td>52</td>
            <td>64</td>
        </tr>
        <tr>
            <td><code><strong>0x6854</strong></code></td>
            <td align="left"><a href="/shdf/maps/ps%20[6854].md">Насосная станция 6854</a></td>
            <td>64</td>
            <td>32</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Логика и интерфейсы</strong></td>
        </tr>
        <tr>
            <td><code><strong>0x7001</strong></code></td>
            <td align="left"><a href="/shdf/maps/logic%20[7001].md">Простая логика тип 1 (дискретная)</a></td>
            <td>4</td>
            <td>24</td>
        </tr>
        <tr>
            <td><code><strong>0x7002</strong></code></td>
            <td align="left"><a href="/shdf/maps/logic%20[7002].md">Простая логика тип 2 (вещественная, пороги)</a></td>
            <td>8</td>
            <td>40</td>
        </tr>
        <tr>
            <td><code><strong>0x7011</strong></code></td>
            <td align="left"><a href="/shdf/maps/sync%20[7011].md">Передача, синхронизация двух битовых переменных в MROM</a></td>
            <td>4</td>
            <td>16</td>
        </tr>
        <tr>
            <td><code><strong>0x7020</strong></code></td>
            <td align="left"><a href="/shdf/maps/sync%20[7020].md">Передача, синхронизация двух вещественных переменных в MROM</a></td>
            <td>16</td>
            <td>8</td>
        </tr>
        <tr>
            <td><code><strong>0x6881</strong></code></td>
            <td align="left"><a href="/shdf/maps/gate%20[6881].md">Шлюз 6881 - RS485</a></td>
            <td>8</td>
            <td>32</td>
        </tr>
        <tr>
            <td><code><strong>0x6891</strong></code></td>
            <td align="left"><a href="/shdf/maps/gate%20[6891].md">Обработчик данных шлюза (преобразование пакета в список переменных)</a></td>
            <td>136</td>
            <td>72</td>
        </tr>
        <tr>
            <td><code><strong>0x6880</strong></code></td>
            <td align="left"><a href="/shdf/maps/ethernet%20[6880].md">Ethernet ретранслятор</a></td>
            <td>8</td>
            <td>20</td>
        </tr>
    </tbody>
</table>
