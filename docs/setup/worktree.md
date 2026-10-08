Тесты в tests/Unit/:

DecisionEngineTest.php — решение approve/review/reject по порогам LTV, включая границы зон (85.0 → review, 85.01 → reject).
LtvCalculatorTest.php — расчёт LTV в процентах (сумма / оценочная стоимость) и исключения при нулевой стоимости или неположительной сумме.
AssessmentServiceTest.php — интеграция сервиса: approve с лимитом = запрошенной сумме, review/reject с нулевым лимитом, корректный возраст авто.
ApplicationValidatorTest.php — валидация заявки: нормализация VIN в верхний регистр, отказ при годе из будущего, минимальной сумме, сбор всех ошибок сразу.
VinValidatorTest.php — формат VIN: 17 символов, регистронезависимость, запрещённые буквы I/O/Q, спецсимволы, пустая строка.
Работаю в папке .../carmoney-lab-ekorolev-smarthorizon/.kilo/worktrees/1-2-3, ветка 1-2-3.

/home/deekor/carmoney/carmoney-lab-ekorolev-smarthorizon                                    b12fe2f [d1/1.2.1-1.2.3-ekorolev-smarthorizon]
/home/deekor/carmoney/carmoney-lab-ekorolev-smarthorizon/.kilo/worktrees/1-2-3              b12fe2f [1-2-3]
/home/deekor/carmoney/carmoney-lab-ekorolev-smarthorizon/.kilo/worktrees/saber-spinosaurus  b12fe2f (detached HEAD)