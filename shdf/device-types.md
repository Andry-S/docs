# Типы (коды) устройств ШДФ

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
            <td>`0x0001`</td>
            <td align="left">Пустое устройство (тест)</td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td>`0x8001`</td>
            <td align="left">Мастер состояния мезонинов</td>
            <td>28</td>
            <td>48</td>
        </tr>
        <tr>
            <td>`0x0002`</td>
            <td align="left">Дискретный вход</td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td>`0x8002`</td>
            <td align="left">Мастер дискретных входов</td>
            <td>N / 8 + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td>`0x0003`</td>
            <td align="left">Дискретных выход</td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td>`0x8003`</td>
            <td align="left">Пустое устройство (тест)</td>
            <td>N / 8 + 4 + N</td>
            <td>8</td>
        </tr>
        <tr>
            <td>`0x0004`</td>
            <td align="left">Аналоговый вход</td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td>`0x8004`</td>
            <td align="left">Мастер аналоговых входов</td>
            <td>12 * N + 4</td>
            <td>8</td>
        </tr>
        <tr>
            <td>`0x0041`</td>
            <td align="left">Аналоговый выход</td>
            <td>32</td>
            <td>24</td>
        </tr>
        <tr>
            <td>`0x0006`</td>
            <td align="left">Мезонин питания СР6761</td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td>`0x6921`</td>
            <td align="left">Мезонин подключения пульта СР6921</td>
            <td>4</td>
            <td>4</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Составные устройства (в составе ссылки на простые либо составные устройства)</strong></td>
        </tr>
        <tr>
            <td>`0x0135`</td>
            <td align="left">Регулятор 6835</td>
            <td>64</td>
            <td>92</td>
        </tr>
        <tr>
            <td>`0x0136`</td>
            <td align="left">Регулятор 6836</td>
            <td>64</td>
            <td>160</td>
        </tr>
        <tr>
            <td>`0x0247`</td>
            <td align="left">Задвижка 6847</td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td>`0x6851`</td>
            <td align="left">Насос 6851</td>
            <td>64</td>
            <td>64</td>
        </tr>
        <tr>
            <td>`0x6852`</td>
            <td align="left">Насосная станция 6852</td>
            <td>52</td>
            <td>64</td>
        </tr>
        <tr>
            <td>`0x6854`</td>
            <td align="left">Насосная станция 6854</td>
            <td>64</td>
            <td>32</td>
        </tr>
        <tr>
            <td colspan="4" align="left"><strong>Логика и интерфейсы</strong></td>
        </tr>
        <tr>
            <td>`0x7001`</td>
            <td align="left">Простая логика тип 1 (дискретная)</td>
            <td>4</td>
            <td>24</td>
        </tr>
        <tr>
            <td>`0x7002`</td>
            <td align="left">Простая логика тип 2 (вещественная, пороги)</td>
            <td>8</td>
            <td>40</td>
        </tr>
        <tr>
            <td>`0x7011`</td>
            <td align="left">Передача, синхронизация двух битовых переменных в MROM</td>
            <td>4</td>
            <td>16</td>
        </tr>
        <tr>
            <td>`0x7020`</td>
            <td align="left">Передача, синхронизация двух вещественных переменных в MROM</td>
            <td>16</td>
            <td>8</td>
        </tr>
        <tr>
            <td>`0x6881`</td>
            <td align="left">Шлюз 6881 - RS485</td>
            <td>8/td>
            <td>32</td>
        </tr>
        <tr>
            <td>`0x6891`</td>
            <td align="left">Обработчик данных шлюза (преобразование пакета в список переменных)</td>
            <td>136</td>
            <td>72</td>
        </tr>
        <tr>
            <td>`0x6880`</td>
            <td align="left">Ethernet ретранслятор</td>
            <td>8</td>
            <td>20</td>
        </tr>
    </tbody>
</table>
