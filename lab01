## Домашнее задание

**Студента группы ИУ8Ц-41**
**Клещинский Иван**


1. Скачайте библиотеку *boost* с помощью утилиты **wget**. Адрес для скачивания `https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz`.
```sh
$ wget https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz

--2025-03-03 10:32:58--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz
Распознаётся sourceforge.net (sourceforge.net)… 104.18.12.149, 104.18.13.149, 2606:4700::6812:c95, ...
Подключение к sourceforge.net (sourceforge.net)|104.18.12.149|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 301 Moved Permanently
Адрес: https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/ [переход]
--2025-03-03 10:32:59--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/
Повторное использование соединения с sourceforge.net:443.
HTTP-запрос отправлен. Ожидание ответа… 301 Moved Permanently
Адрес: https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/download [переход]
--2025-03-03 10:32:59--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/download
Повторное использование соединения с sourceforge.net:443.
HTTP-запрос отправлен. Ожидание ответа… 302 Found
Адрес: https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?ts=gAAAAABnxcutW4MZM3PQ6psZEfaDkTmJYwUiUHLlloWazXEqhkoxvnylBFx0Z0okLfqGi4SMUnKODS6D1g47_mnXDF2cNxi1Pw%3D%3D&use_mirror=unlimited&r= [переход]
--2025-03-03 10:33:00--  https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?ts=gAAAAABnxcutW4MZM3PQ6psZEfaDkTmJYwUiUHLlloWazXEqhkoxvnylBFx0Z0okLfqGi4SMUnKODS6D1g47_mnXDF2cNxi1Pw%3D%3D&use_mirror=unlimited&r=
Распознаётся downloads.sourceforge.net (downloads.sourceforge.net)… 104.18.12.149, 104.18.13.149, 2606:4700::6812:d95, ...
Подключение к downloads.sourceforge.net (downloads.sourceforge.net)|104.18.12.149|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 302 Found
Адрес: https://unlimited.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?viasf=1 [переход]
--2025-03-03 10:33:01--  https://unlimited.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?viasf=1
Распознаётся unlimited.dl.sourceforge.net (unlimited.dl.sourceforge.net)… 185.119.90.247
Подключение к unlimited.dl.sourceforge.net (unlimited.dl.sourceforge.net)|185.119.90.247|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 200 OK
Длина: 111710205 (107M) [application/x-gzip]
Сохранение в: «boost_1_69_0.tar.gz»

boost_1_69_0.tar.gz 100%[================>] 106,53M  1,99MB/s    за 69s     

2025-03-03 10:34:15 (1,54 MB/s) - «boost_1_69_0.tar.gz» сохранён [111710205/111710205]

```
2. Разархивируйте скачанный файл в директорию `~/boost_1_69_0`
```sh
$ tar -xzvf boost_1_69_0.tar.gz -C /workspace
[Результаты](https://gist.github.com/METEOPuT/c004a78affa66e1461ae626ed2ce6abf)
```
3. Подсчитайте количество файлов в директории `~/boost_1_69_0` **не включая** вложенные директории.
```sh
$ ls -l /workspace/boost_1_69_0 | grep ^- | wc -l
12
```
4. Подсчитайте количество файлов в директории `~/boost_1_69_0` **включая** вложенные директории.
```sh
$ find /workspace/boost_1_69_0 -type f | wc -l
61191
```
5. Подсчитайте количество заголовочных файлов, файлов с расширением `.cpp`, сколько остальных файлов (не заголовочных и не `.cpp`).
```sh
$ find /workspace/boost_1_69_0 -type f \( -name "*.h" -o -name "*.hpp" \) | wc -l
15208
$ find /workspace/boost_1_69_0 -type f -name "*.cpp" | wc -l
13774
$ find /workspace/boost_1_69_0 -type f ! \( -name "*.h" -o -name "*.hpp" -o -name "*.cpp" \) | wc -l
32209
```
6. Найдите полный пусть до файла `any.hpp` внутри библиотеки *boost*.
```sh
$ find /workspace/boost_1_69_0 -type f -name "any.hpp"
/workspace/boost_1_69_0/boost/any.hpp
/workspace/boost_1_69_0/boost/type_erasure/any.hpp
/workspace/boost_1_69_0/boost/proto/detail/any.hpp
/workspace/boost_1_69_0/boost/spirit/home/support/algorithm/any.hpp
/workspace/boost_1_69_0/boost/xpressive/detail/utility/any.hpp
/workspace/boost_1_69_0/boost/hana/any.hpp
/workspace/boost_1_69_0/boost/hana/fwd/any.hpp
/workspace/boost_1_69_0/boost/fusion/algorithm/query/any.hpp
/workspace/boost_1_69_0/boost/fusion/algorithm/query/detail/any.hpp
/workspace/boost_1_69_0/boost/fusion/include/any.hpp
```
7. Выведите в консоль все файлы, где упоминается последовательность `boost::asio`.
```sh
$ grep -r "boost::asio" /workspace/boost_1_69_0 > /workspace/reports/zad1.7
[Результаты](https://gist.github.com/METEOPuT/430bdf6e3944a422ac2168dd146899cc)
```
8. Скомпилирутйе *boost*. Можно воспользоваться [инструкцией](https://www.boost.org/doc/libs/1_61_0/more/getting_started/unix-variants.html#or-build-custom-binaries) или [ссылкой](https://codeyarns.com/2017/01/24/how-to-build-boost-on-linux/).
```sh
$ ./bootstrap.sh
$ ./b2
[Компиляция](https://gist.github.com/METEOPuT/7eb7df4d53baf0f63462f23dc7272855)
$ sudo ./b2 install
$ ls /usr/local/lib | grep boost
libboost_atomic.a
libboost_atomic.so
libboost_atomic.so.1.69.0
libboost_chrono.a
libboost_chrono.so
libboost_chrono.so.1.69.0
libboost_container.a
libboost_container.so
libboost_container.so.1.69.0
libboost_context.a
libboost_context.so
libboost_context.so.1.69.0
libboost_contract.a
libboost_contract.so
libboost_contract.so.1.69.0
libboost_date_time.a
libboost_date_time.so
libboost_date_time.so.1.69.0
libboost_exception.a
libboost_fiber.a
libboost_fiber.so
libboost_fiber.so.1.69.0
libboost_filesystem.a
libboost_filesystem.so
libboost_filesystem.so.1.69.0
libboost_graph.a
libboost_graph.so
libboost_graph.so.1.69.0
libboost_iostreams.a
libboost_iostreams.so
libboost_iostreams.so.1.69.0
libboost_prg_exec_monitor.a
libboost_prg_exec_monitor.so
libboost_prg_exec_monitor.so.1.69.0
libboost_program_options.a
libboost_program_options.so
libboost_program_options.so.1.69.0
libboost_random.a
libboost_random.so
libboost_random.so.1.69.0
libboost_regex.a
libboost_regex.so
libboost_regex.so.1.69.0
libboost_serialization.a
libboost_serialization.so
libboost_serialization.so.1.69.0
libboost_stacktrace_addr2line.a
libboost_stacktrace_addr2line.so
libboost_stacktrace_addr2line.so.1.69.0
libboost_stacktrace_backtrace.a
libboost_stacktrace_backtrace.so
libboost_stacktrace_backtrace.so.1.69.0
libboost_stacktrace_basic.a
libboost_stacktrace_basic.so
libboost_stacktrace_basic.so.1.69.0
libboost_stacktrace_noop.a
libboost_stacktrace_noop.so
libboost_stacktrace_noop.so.1.69.0
libboost_system.a
libboost_system.so
libboost_system.so.1.69.0
libboost_test_exec_monitor.a
libboost_timer.a
libboost_timer.so
libboost_timer.so.1.69.0
libboost_unit_test_framework.a
libboost_unit_test_framework.so
libboost_unit_test_framework.so.1.69.0
libboost_wave.a
libboost_wserialization.a
libboost_wserialization.so
libboost_wserialization.so.1.69.0
```
9. Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию `~/boost-libs`.
```sh
$ mkdir ~/boost-libs 
$ mv /usr/local/lib/libboost_*.a ~/boost-libs
$ ls ~/boost-libs
libboost_atomic.a      libboost_graph.a                 libboost_stacktrace_basic.a
libboost_chrono.a      libboost_iostreams.a             libboost_stacktrace_noop.a
libboost_container.a   libboost_prg_exec_monitor.a      libboost_system.a
libboost_context.a     libboost_program_options.a       libboost_test_exec_monitor.a
libboost_contract.a    libboost_random.a                libboost_timer.a
libboost_date_time.a   libboost_regex.a                 libboost_unit_test_framework.a
libboost_exception.a   libboost_serialization.a         libboost_wave.a
libboost_fiber.a       libboost_stacktrace_addr2line.a  libboost_wserialization.a
libboost_filesystem.a  libboost_stacktrace_backtrace.a
```
10. Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
```sh
$ du -ah ~/boost-libs
4,5M    /home/kali/boost-libs/libboost_wave.a
232K    /home/kali/boost-libs/libboost_chrono.a
52K     /home/kali/boost-libs/libboost_timer.a
828K    /home/kali/boost-libs/libboost_graph.a
276K    /home/kali/boost-libs/libboost_iostreams.a
3,1M    /home/kali/boost-libs/libboost_regex.a
4,0K    /home/kali/boost-libs/libboost_stacktrace_noop.a
320K    /home/kali/boost-libs/libboost_contract.a
20K     /home/kali/boost-libs/libboost_context.a
2,2M    /home/kali/boost-libs/libboost_test_exec_monitor.a
4,0K    /home/kali/boost-libs/libboost_exception.a
4,0K    /home/kali/boost-libs/libboost_atomic.a
80K     /home/kali/boost-libs/libboost_random.a
152K    /home/kali/boost-libs/libboost_date_time.a
1,2M    /home/kali/boost-libs/libboost_serialization.a
776K    /home/kali/boost-libs/libboost_wserialization.a
16K     /home/kali/boost-libs/libboost_stacktrace_basic.a
232K    /home/kali/boost-libs/libboost_fiber.a
2,2M    /home/kali/boost-libs/libboost_unit_test_framework.a
404K    /home/kali/boost-libs/libboost_filesystem.a
4,0K    /home/kali/boost-libs/libboost_system.a
20K     /home/kali/boost-libs/libboost_stacktrace_backtrace.a
152K    /home/kali/boost-libs/libboost_container.a
208K    /home/kali/boost-libs/libboost_prg_exec_monitor.a
36K     /home/kali/boost-libs/libboost_stacktrace_addr2line.a
1,5M    /home/kali/boost-libs/libboost_program_options.a
19M     /home/kali/boost-libs
```
11. Найдите *топ10* самых "тяжёлых".
```sh
$ du -ah ~/boost-libs | grep -v '/$' | sort -hr | head -10
19M     /home/kali/boost-libs
4,5M    /home/kali/boost-libs/libboost_wave.a
3,1M    /home/kali/boost-libs/libboost_regex.a
2,2M    /home/kali/boost-libs/libboost_unit_test_framework.a
2,2M    /home/kali/boost-libs/libboost_test_exec_monitor.a
1,5M    /home/kali/boost-libs/libboost_program_options.a
1,2M    /home/kali/boost-libs/libboost_serialization.a
828K    /home/kali/boost-libs/libboost_graph.a
776K    /home/kali/boost-libs/libboost_wserialization.a
404K    /home/kali/boost-libs/libboost_filesystem.a
```
