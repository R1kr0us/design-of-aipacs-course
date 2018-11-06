# Проектирование АСОиУ
## Курс проектирования автоматизированных систем обработки информации и управления
Данный репозиторий предназначен для хранения материалов курса и результатов выполнения лабораторных работ. Это описание будет дополняться постепенно по мере проведения лекций и лабораторных работ.

### Структура репозитория
В репозитории имеется папка **Labs** для всех лабораторных работ. В неё будут постепенно добавляться отдельные папки для каждой лабораторной работы (**Lab_#**), в корень каждой из которых необходимо помещать свои результаты лабораторной работы: созданные файлы, протоколы и т.п. Также в каждой из них может быть папка с материалами для лабораторной работы (**Materials**), например, лекциями, шпаргалками, исходниками и т.п.

Например, сейчас уже имеется папка **Lab_1**, в корень которой нужно будет поместить .bpmn-файл своей диаграммы BPMN и файл протокола. В ней также имеется папка **Materials** с файлом лекции для лабораторной работы.

Также в репозитории имеется Excel-таблица с данными о посещаемости лабораторных работ и отметками о выполнении домашних заданий, которая будет обновляться по мере проведения работ и проверки результатов.

### Порядок работы с репозиторием
Каждому магистранту необходимо стать участником данного репозитория, каждому будет выслано приглашение, если указанный почтовый ящик привязан к аккаунту GitHub. Ветка master предназначена только для преподавателя, он в неё будет выкладывать задания и прочие материалы. Каждый магистрант должен создать для себя отдельную ветку от ветки **master**, начиная с последнего имеющегося коммита, назвав её своей фамилией на латинице (например, **Ivanov**). В свою ветку необходимо коммитить результаты выполнения лабораторных работ (файлы исходного кода, диаграммы, протоколы) в папки лабораторных (можно создавать свои подпапки для различных групп файлов). Периодически необходимо сливать ветку master со своей веткой для получения материалов и заданий для новых лабораторных. **Сливать свою ветку в master НЕ НУЖНО!** **Делать коммиты в master НЕ НУЖНО!** Протоколы лучше сохранять в файлы формата .pdf.

Советую также подобрать себе красивый GUI для работы с Git, чтобы проще ориентироваться в ветках. [Вот, хорошая подборка](https://git-scm.com/download/gui/windows), например GitKraken - очень красивый, а SourceTree - простой и один интерфейс для Git и Hg. Но некоторые могут лагать на разных системах, так что выбирайте.

### Описание лабораторных работ
#### Лабораторная работа №1: Диаграммы BPMN
Данная лабораторная работа посвящена нотации моделирования бизнес-процессов BPMN. В папке с материалами имеется короткая лекция, которая была рассказана на лабораторной.

**Задание на дом:** необходимо разработать модель некоторого бизнес-процесса, связанного с тематикой своей магистерской диссертации или непосредственно для неё. Необходимо закоммитить в репозиторий .bpmn-файл своей диаграммы, а также документ отчёта, в котором нужно словесно описать данный бизнес-процесс, прокомментировать его этапы, возможно, добавить какие-то примечания к диаграмме, чтобы преподавателю было проще положительно оценить её. Программы для моделирования диаграмм и прочая дополнительная информация описана в лекции для лабораторной.

**Список заданий** для тех, кто не придумал себе собственное (варианты совпадать не должны, но могут вами модифицироваться, улучшаться или упрощаться, дополняться). Эти же варианты могут быть использованы для создания **DMN-диаграмм лабораторной работы №2**:
1. процесс сборки робота для различных промышленных нужд (выявление требований, выбор технологий передвижения, выбор манипуляторов, выявление наиболее удобного способа управления в зависимости от задач, сборка робота, тестирование и т.д.);
1. процесс подборки и размещения системы автоматического освещения в здании со сбором данных о своей работе и потреблении электроэнергии (выявление требований, выбор датчиков и способа управления, монтаж датчиков, светильников, подключение всего вместе и т.д.);
1. процесс создания группы собственных устройств (датчиков), работающих как Internet of Things (взаимодействующих друг с другум и с ПК) для каких-либо нужд (подбор компонентов, изготовление корпуса на 3d-принтере, выбор способа взаимодействия, сборка, написание ПО, тестирование, улучшение и т.п.); 
1.процесс взаимодействия созданных датчиков, описанных в задании выше (передача данных и иное взаимодействие, оповещения пользователей, обработка критических ситуаций, обновление ПО и т.д.);
1. процесс автоматизированного управления дроном (летающим, ползающим и т.д.), например, пылесосом, с наличием базы, с которой он отправляется на задание и возвращается, выполняет какие-то действия, с обработкой критических ситуаций и оповещением пользователя;
1. процесс автоматизированного управления каким-либо производством или процессом, например, нагревательным котлом для душевых, который сам нагревает воду и поддерживает температуру, наполняет по мере необходимости, отключается при неиспользовании, обрабатывает критические ситуации, вроде, выключения света, использует альтернативные источники тепла и т.п.;
1. процесс изготовления какого-либо изделия на производстве, например инструмента (доставка сырья, подготовка сырья, изготовления 1-й, 2-й, 3-й детали, сборка, обработка, упаковка, оценка качества и т.п., обработка критических ситуаций);
1. процесс подбора экзоскелета для человека с какими-то ограничениями (выбор типа экзоскелета, выбор способа крепления, компонентов, питания, ПО, сложности конструкции и т.п.).

#### Лабораторная работа №2: Диаграммы DMN
Данная лабораторная работа посвящена нотации моделирования процесса принятия решений DMN. В папке с материалами имеется короткая лекция, которая была рассказана на лабораторной. Также в папке с материалами к лабораторной есть статья 2018-го года о расширении нотации DMN для использования больших данных. Советую ознакомиться, как с примером использования данной нотации, очень интересно.

**Задание на дом:** необходимо разработать модель принятия решений, связанную с тематикой своей магистерской диссертации или непосредственно для неё, или же по собственной теме или из списка выше в задании для лабораторной работы №1. Данная диаграмма может быть одним из блоков BPMN-диаграммы предыдущей лабораторной. Необходимо закоммитить в репозиторий .dmn-файл своей диаграммы, а также документ отчёта, в котором нужно словесно описать предметную область вашей диаграммы принятия решений, прокомментировать её этапы, возможно, добавить какие-то примечания к диаграмме.

#### Лабораторная работа №3: Формирование требований к АСОиУ
Данная лабораторная работа посвящена различным методам описания требований к своему проекту, программному продукту. 

**Задание на дом:**
1. описать свой проект или программный продукт по спецификации **Vision & Scope** (шаблон документа находится в папке с материалами, ссылки на помощь в оформлении находится в презентации к лабораторной);
1. описать свой проект или программный продукт по спецификации **System Requirements Specification (SRS)** (шаблон документа также находится в папке с материалами, там же находится документ с методикой его составления и образец).
Желательно реализовать диаграмму Use-Case или диаграмму последовательности, а также описать *одно предложение* для своего проекта.

#### Лабораторная работа №4. Разработка ТЗ
Лабораторная работа посвящена формированию требований к АС, разработке концепции АС. Техническое задание. Эскизный проект. Технический проект. Рабочая документация.
Главный источник шаблонов: http://www.rugost.com/

**Материалы:**
* [Стандарты и шаблоны для ТЗ на разработку ПО](https://habr.com/post/328822/)
* [Разработка технического задания. Часть 1. Что это такое, зачем оно нужно, с чего начать и как должно выглядеть?](https://infostart.ru/public/123632/)
* [Как разработать Техническое задание. Часть 2. Виды работ при сборе требований к системе учета и информации для описания бизнес-процессов](https://habr.com/post/147858/)
* [Техническое задание: как уберечь себя от ошибок и рисков](https://habr.com/post/139835/)
* [Что такое «хорошее» ТЗ на сайт?](https://habr.com/post/5556/)

