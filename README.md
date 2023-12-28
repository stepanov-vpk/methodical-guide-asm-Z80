# Краткое методическое пособие по ассемблеру Z80

## Основные понятия языка ассемблера

`Язык ассемблера` - это низкоуровневый язык программирования, который предоставляет удобные средства для написания программ, управляющих аппаратными ресурсами компьютера.

Программы на языке ассемблера представляют собой набор инструкций (команд), каждая из которых соответствует определенной операции, выполняемой процессором. Для каждой компьютерной архитектуры существует свой собственный набор команд и правил написания программ на языке ассемблера.

Перейдём к рассмотрению основных понятий языка ассемблера.

#### 1. Инструкции

`Мнемоника` - это команда, либо основная операция, которая выполняется процессором. Большинство мнемоник представляют собой сокращенную версию слова. Например: LD - Load, INC - Increment

#### 2. Регистры процессора

`Регистр` - это некоторое хранилище данных, которое используется для временного хранения информации, промежуточных результатов и выполнения операций.

Основные регистры микропроцессора Z80 включают в себя следующие:
1. Регистры общего назначения (главные регистры):
   - Регистры A, B, C, D, E, H, L - каждый из них состоит из 8 бит и используется для выполнения различных арифметических и логических операций;
   - Регистр F - состоит из 8 бит и используется для хранения флагов состояния процессора, таких как флаги переноса, нуля, переноса через знак и других.
2. Специализированные регистры:
   - Регистр SP (Stack Pointer) - 16-битный регистр, который указывает на текущую вершину стека и используется для управления стековыми операциями;
   - Регистр PC (Program Counter) - 16-битный регистр, который указывает на адрес следующей инструкции, которая должна быть выполнена;
   - Регистр IX и IY - 16-битные индексные регистры, которые используются для адресации данных в памяти.

### 3. Набор команд микропроцессора

Микропроцессор Z80 имеет обширный набор команд ассемблера, которые позволяют программистам выполнять различные операции с данными, управлять памятью и регистрами процессора, а также управлять потоком выполнения программы. Вот некоторые из основных команд ассемблера для Z80:

1. Арифметические операции:
   - ADD, SUB, ADC, SBC - команды для сложения, вычитания с учетом переноса и без него
   - INC, DEC - команды для инкрементирования и декрементирования регистров и ячеек памяти

2. Логические операции:
   - AND, OR, XOR - битовые логические операции
   - CPL, CCF, SCF - команды для инвертирования битов, управления флагами

3. Управление потоком выполнения:
   - JP, JR - команды для безусловного и условного перехода
   - CALL, RET - команды для вызова и возврата из подпрограммы
   - RST - команда для вызова прерывания

4. Управление памятью и регистрами:
   - LD - команда для загрузки данных в регистры и ячейки памяти
   - PUSH, POP - команды для записи и чтения данных из стека
   - LDAX, STAX - команды для доступа к регистровым парам

5. Другие команды:
   - HALT - команда для перевода процессора в режим ожидания
   - NOP - команда No Operation, означает отсутствие операции

Регистры микропроцессора Z80 являются основными элементами его архитектуры и обеспечивают полную функциональность процессора для выполнения различных операций с данными и управления программой.

Каждая команда ассемблера микропроцессора Z80 представляет собой определенную операцию, которую процессор может выполнить. Программисты используют эти команды для написания программ для Z80, управления данными, выполнения вычислений и управления потоком выполнения программы.
