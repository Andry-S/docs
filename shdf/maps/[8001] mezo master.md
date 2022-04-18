# Карта памяти устройства `Мастер состояния мезонинов [8001]`

## Ссылки

- [Документация ШДФ](/shdf/)
  - [Карта памяти заданных типов устройств ШДФ](/shdf/devices-map.md)
  - [Типы (коды) устройств ШДФ](/shdf/device-types.md)
  - [Карты памяти устройств ШДФ:](/shdf/maps/)
    - [`[0002] Дискретный вход`](/shdf/maps/[0002]%20di.md)
    - [`[0003] Дискретный выход`](/shdf/maps/[0003]%20do.md)
    - [`[0004] Аналоговый вход`](/shdf/maps/[0004]%20ai.md)
    - [`[0041] Аналоговый выход`](/shdf/maps/[0041]%20ao.md)
    - [`[0135] Регулятор 6835`](/shdf/maps/[0135]%20reg.md)
    - [`[0136] Регулятор 6836`](/shdf/maps/[0136]%20reg.md)
    - [`[0247] Задвижка 6847`](/shdf/maps/[0247]%20valve.md)
    - [`[6851] Насос 6851`](/shdf/maps/[6851]%20pump.md)
    - [`[6852] Насосная станция 6852`](/shdf/maps/[6852]%20ps.md)
    - [`[6853] Насос 6853`](/shdf/maps/pump%20[6853]%20.md)
    - [`[6854] Насосная станция 6854`](/shdf/maps/[6854]%20ps.md)
    - [`[6880] Ethernet ретранслятор`](/shdf/maps/[6880]%20ethernet.md)
    - [`[6881] Шлюз 6881 - RS485`](/shdf/maps/[6881]%20gate.md)
    - [`[6891] Обработчик данных шлюза (преобразование пакета в список переменных)`](/shdf/maps/[6891]%20gate.md)
    - [`[7001] Простая логика тип 1 (дискретная)`](/shdf/maps/[7001]%20logic.md)
    - [`[7002] Простая логика тип 2 (вещественная, пороги)`](/shdf/maps/[7002]%20logic.md)
    - [`[7011] Передача, синхронизация двух битовых переменных в MROM`](/shdf/maps/[7011]%20sync.md)
    - [`[7020] Передача, синхронизация двух вещественных переменных в MROM`](/shdf/maps/[7020]%20sync.md)
    - [**`[8001] Мастер состояния мезонинов`**](/shdf/maps/[80001]%20mezo%20master.md)
    - [`[8002] Мастер дискретных входов`](/shdf/maps/[8002]%20mdi.md)
    - [`[8003] Мастер дискретных выходов`](/shdf/maps/[8003]%20mdo.md)
    - [`[8004] Мастер аналоговых входов`](/shdf/maps/[8004]%20mai.md)
    - [`???[0006] Мезонин питания СР6761`](/shdf/maps/[0006]%20pu.md)
    - [`???[6921] Мезонин подключения пульта СР6921`](/shdf/maps/[6921]%20rc.md)

## Карта памяти `MROM`

<table summary="Карта памяти `MROM`" border="1">
    <tbody valign="center" align="center">
        <tr>
            <td><strong>Индекс</strong></td>
            <td><strong>Регистр</strong></td>
            <td><strong>Смещение</strong></td>
            <td><strong>Бит</strong></td>
            <td align="left"><strong>Назначение</strong></td>
            <td align="left"><strong>Примечание</strong></td>
        </tr>
        <tr>
            <td><code>MROM:001</code></td>
            <td rowspan="2">0</td>
            <td>0</td>
            <td>BYTE</td>
            <td align="left">Номер опрашиваемой колодки</td>
            <td>1...4</td>
        </tr>
        <tr>
            <td><code>MROM:002</code></td>
            <td>1</td>
            <td>BYTE</td>
            <td align="left">Команда управления</td>
            <td>—</td>
        </tr>
        <tr>
            <td><code>MROM:003</code></td>
            <td rowspan="16"><i>1</i></td>
            <td rowspan="8">2</td>
            <td>0</td>
            <td align="left">Процессор в работе (1 – работа)</td>
            <td rowspan="8">Байт состояния процессора 1</td>
        </tr>
        <tr>
            <td><code>MROM:004</code></td>
            <td><i>1</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:005</code></td>
            <td><i>2</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:006</code></td>
            <td><i>3</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:007</code></td>
            <td><i>4</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:008</code></td>
            <td><i>5</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:009</code></td>
            <td><i>6</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:010</code></td>
            <td><i>7</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:011</code></td>
            <td rowspan="8">3</td>
            <td>0</td>
            <td align="left">Сигнал "Запись в ЕЕПРОМ"</td>
            <td rowspan="8">Байт состояния процессора 2</td>
        </tr>
        <tr>
            <td><code>MROM:012</code></td>
            <td><i>1</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:013</code></td>
            <td><i>2</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:014</code></td>
            <td><i>3</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:015</code></td>
            <td><i>4</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:016</code></td>
            <td><i>5</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:017</code></td>
            <td><i>6</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:018</code></td>
            <td><i>7</i></td>
            <td align="left"><i>Резерв</i></td>
        </tr>
        <tr>
            <td><code>MROM:019</code></td>
            <td rowspan="2">2</td>
            <td>4</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонинов М1-1, М2-1</td>
            <td rowspan="2" align="left">биты 0-3 – M1-1,<br>биты 4-7 – М2-1</td>
        </tr>
        <tr>
            <td><code>MROM:020</code></td>
            <td>5</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонинов М1-2, М2-2</td>
        </tr>
        <tr>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
        </tr>
        <tr>
            <td><code>MROM:039</code></td>
            <td rowspan="2">12</td>
            <td>24</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонинов М1-21, М2-21</td>
            <td rowspan="2" align="left">биты 0-3 – M1-21,<br>биты 4-7 – М2-21</td>
        </tr>
        <tr>
            <td><code>MROM:040</code></td>
            <td>25</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонинов М1-22, М2-22</td>
        </tr>
        <tr>
            <td><code>MROM:041</code></td>
            <td rowspan="2">13</td>
            <td><i>26</i></td>
            <td><i>BYTE</i></td>
            <td align="left"><i>Резерв</i></td>
            <td><i>—</i></td>
        </tr>
        <tr>
            <td><code>MROM:042</code></td>
            <td>27</td>
            <td><i>BYTE</i></td>
            <td align="left"><i>Резерв</i></td>
            <td><i>—</i></td>
        </tr>
    </tbody>
</table>

## Карта памяти `EEPROM`

<table summary="Карта памяти `MROM`" border="1">
    <tbody valign="center" align="center">
        <tr>
            <td><strong>Индекс</strong></td>
            <td><strong>Регистр</strong></td>
            <td><strong>Смещение</strong></td>
            <td><strong>Бит</strong></td>
            <td align="left"><strong>Назначение</strong></td>
            <td align="left"><strong>Примечание</strong></td>
        </tr>
        <tr>
            <td><code>EEPROM:001</code></td>
            <td rowspan="2">0</td>
            <td>0</td>
            <td>BYTE</td>
            <td align="left">Номер опрашиваемой колодки</td>
            <td>1...4</td>
        </tr>
        <tr>
            <td><code>EEPROM:002</code></td>
            <td><i>1</i></td>
            <td><i>BYTE</i></td>
            <td align="left"><i>Резерв</i></td>
            <td>—</td>
        </tr>
        <tr>
            <td><code>EEPROM:003</code></td>
            <td rowspan="2"><i>1</i></td>
            <td><i>2</i></td>
            <td><i>BYTE</i></td>
            <td align="left"><i>Резерв</i></td>
            <td>—</td>
        </tr>
        <tr>
            <td><code>EEPROM:004</code></td>
            <td><i>3</i></td>
            <td><i>BYTE</i></td>
            <td align="left"><i>Резерв</i></td>
            <td>—</td>
        </tr>
        <tr>
            <td><code>EEPROM:005</code></td>
            <td rowspan="2">2</td>
            <td>4</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М1-1</td>
            <td rowspan="10" align="left">Коды типов мезонинов:<br><code>0x11</code> – СР6711<br><code>0x13</code> – СР6713<br><code>0x23</code> – СР6723<br><code>0x24</code> – СР6724<br><code>0x25</code> – СР6725<br><code>0x26</code> – СР6726<br><code>0x31</code> – СР6731<br><code>0x32</code> – СР6732<br><code>0x41</code> – СР6741<br><code>0x51</code> – СР6751<br><code>0x61</code> – СР6761</td>
        </tr>
        <tr>
            <td><code>EEPROM:006</code></td>
            <td>5</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М1-2</td>
        </tr>
        <tr>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
        </tr>
        <tr>
            <td><code>EEPROM:027</code></td>
            <td rowspan="2">13</td>
            <td>26</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М1-21</td>
        </tr>
        <tr>
            <td><code>EEPROM:028</code></td>
            <td>27</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М1-22</td>
        </tr>
        <tr>
            <td><code>EEPROM:029</code></td>
            <td rowspan="2">14</td>
            <td>28</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М2-1</td>
        </tr>
        <tr>
            <td><code>EEPROM:030</code></td>
            <td>29</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М2-2</td>
        </tr>
        <tr>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
            <td>...</td>
        </tr>
        <tr>
            <td><code>MROM:047</code></td>
            <td rowspan="2">23</td>
            <td>46</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М2-21</td>
        </tr>
        <tr>
            <td><code>MROM:048</code></td>
            <td>47</td>
            <td>BYTE</td>
            <td align="left">Состояние мезонина М2-22</td>
        </tr>
    </tbody>
</table>
