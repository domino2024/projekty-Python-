import random

def run_quiz():
    # Słownik pytań – wszystkie pytania dla każdego poziomu trudności i w każdej wersji językowej
    quizzes = {
        "pl": {
            "easy": [
                {
                    "pytanie": "Co to jest testowanie?",
                    "choices": {
                        "a": "Pisanie kodu.",
                        "b": "Sprawdzanie oprogramowania.",
                        "c": "Tworzenie dokumentacji.",
                        "d": "Optymalizacja sprzętu."
                    },
                    "poprawna": "b",
                    "explanation": "Testowanie polega na weryfikacji, czy oprogramowanie działa zgodnie z oczekiwaniami."
                },
                {
                    "pytanie": "Czym są testy jednostkowe?",
                    "choices": {
                        "a": "Testy pojedynczych funkcji lub modułów.",
                        "b": "Testy całego systemu.",
                        "c": "Testy interfejsu użytkownika.",
                        "d": "Testy wydajnościowe."
                    },
                    "poprawna": "a",
                    "explanation": "Testy jednostkowe sprawdzają działanie pojedynczych elementów oprogramowania."
                },
                {
                    "pytanie": "Czym jest testowanie automatyczne?",
                    "choices": {
                        "a": "Testowanie ręczne.",
                        "b": "Testowanie przy użyciu narzędzi.",
                        "c": "Testowanie z wykorzystaniem analizy statycznej.",
                        "d": "Testowanie oparte na monitorowaniu aplikacji w czasie rzeczywistym."
                    },
                    "poprawna": "b",
                    "explanation": "Automatyzacja testów wykorzystuje narzędzia do uruchamiania testów bez interwencji człowieka."
                },
                {
                    "pytanie": "Co oznacza termin 'regresja' w testowaniu?",
                    "choices": {
                        "a": "Testowanie nowych funkcji.",
                        "b": "Powtórne testowanie po wprowadzeniu zmian.",
                        "c": "Testowanie interfejsu.",
                        "d": "Testowanie wydajnościowe."
                    },
                    "poprawna": "b",
                    "explanation": "Testy regresyjne sprawdzają, czy zmiany w kodzie nie wpłynęły negatywnie na działanie systemu."
                },
                {
                    "pytanie": "Czym są testy integracyjne?",
                    "choices": {
                        "a": "Testy współdziałania modułów systemu.",
                        "b": "Testy jednostkowe.",
                        "c": "Testy interfejsu.",
                        "d": "Testy wydajnościowe."
                    },
                    "poprawna": "a",
                    "explanation": "Testy integracyjne weryfikują, czy poszczególne moduły współpracują ze sobą poprawnie."
                },
                {
                    "pytanie": "Co to jest testowanie eksploracyjne?",
                    "choices": {
                        "a": "Testowanie według ustalonego skryptu.",
                        "b": "Spontaniczne testowanie bez scenariuszy.",
                        "c": "Testowanie obciążeniowe.",
                        "d": "Testy jednostkowe."
                    },
                    "poprawna": "b",
                    "explanation": "Exploracyjne testowanie polega na poszukiwaniu błędów bez uprzednio przygotowanych przypadków testowych."
                },
                {
                    "pytanie": "Czym jest testowanie manualne?",
                    "choices": {
                        "a": "Testowanie z wykorzystaniem narzędzi.",
                        "b": "Testowanie wykonywane przez człowieka.",
                        "c": "Automatyczne testowanie.",
                        "d": "Testy integracyjne."
                    },
                    "poprawna": "b",
                    "explanation": "Testowanie manualne oznacza wykonywanie testów przez osobę."
                },
                {
                    "pytanie": "Co to jest bug?",
                    "choices": {
                        "a": "Nowa funkcjonalność.",
                        "b": "Błąd w oprogramowaniu.",
                        "c": "Fragment kodu.",
                        "d": "Rodzaj testu."
                    },
                    "poprawna": "b",
                    "explanation": "Bug to błąd lub usterka w oprogramowaniu."
                },
                {
                    "pytanie": "Dlaczego dokumentacja testów jest ważna?",
                    "choices": {
                        "a": "Ułatwia powtarzanie testów.",
                        "b": "Przyspiesza pisanie kodu.",
                        "c": "Nie jest istotna.",
                        "d": "Zwiększa liczbę błędów."
                    },
                    "poprawna": "a",
                    "explanation": "Dokumentacja umożliwia odtworzenie i analizę przeprowadzonych testów."
                },
                {
                    "pytanie": "Co to jest przypadek testowy?",
                    "choices": {
                        "a": "Scenariusz do przetestowania funkcji.",
                        "b": "Raport o błędzie.",
                        "c": "Fragment kodu.",
                        "d": "Element dokumentacji."
                    },
                    "poprawna": "a",
                    "explanation": "Przypadek testowy opisuje scenariusz, według którego przeprowadza się test."
                }
            ],
            "medium": [
                {
                    "pytanie": "Co to jest testowanie regresyjne?",
                    "choices": {
                        "a": "Testowanie wydajnościowe.",
                        "b": "Ponowne testowanie po zmianach w kodzie.",
                        "c": "Testowanie interfejsu użytkownika.",
                        "d": "Testowanie bezpieczeństwa."
                    },
                    "poprawna": "b",
                    "explanation": "Testy regresyjne sprawdzają, czy zmiany nie wprowadziły nowych błędów."
                },
                {
                    "pytanie": "Jakie są zalety automatyzacji testów?",
                    "choices": {
                        "a": "Większa powtarzalność testów.",
                        "b": "Zwiększenie kosztów.",
                        "c": "Bardziej skomplikowana konfiguracja.",
                        "d": "Wymaga więcej czasu manualnego."
                    },
                    "poprawna": "a",
                    "explanation": "Automatyzacja pozwala na szybsze i bardziej spójne wykonywanie testów."
                },
                {
                    "pytanie": "Czym są testy obciążeniowe?",
                    "choices": {
                        "a": "Testy sprawdzające działanie systemu przy dużym ruchu.",
                        "b": "Testy interfejsu.",
                        "c": "Testy regresyjne.",
                        "d": "Testy jednostkowe."
                    },
                    "poprawna": "a",
                    "explanation": "Testy obciążeniowe mierzą wydajność systemu pod dużym obciążeniem."
                },
                {
                    "pytanie": "Które narzędzie jest popularne przy testowaniu automatycznym?",
                    "choices": {
                        "a": "Selenium",
                        "b": "Photoshop",
                        "c": "Microsoft Word",
                        "d": "Excel"
                    },
                    "poprawna": "a",
                    "explanation": "Selenium to jedno z najczęściej używanych narzędzi do automatyzacji testów aplikacji webowych."
                },
                {
                    "pytanie": "Co oznacza skrót CI/CD?",
                    "choices": {
                        "a": "Continuous Integration / Continuous Deployment",
                        "b": "Central Integration / Continuous Development",
                        "c": "Continuous Inspection / Continuous Documentation",
                        "d": "Critical Integration / Critical Deployment"
                    },
                    "poprawna": "a",
                    "explanation": "CI/CD to praktyki umożliwiające ciągłą integrację i wdrażanie zmian."
                },
                {
                    "pytanie": "Czym jest testowanie oparte na ryzyku?",
                    "choices": {
                        "a": "Testowanie wszystkich funkcji równomiernie.",
                        "b": "Skupienie testów na obszarach o wysokim ryzyku awarii.",
                        "c": "Testowanie oparte na analizie pokrycia kodu.",
                        "d": "Testowanie interfejsu."
                    },
                    "poprawna": "b",
                    "explanation": "Testowanie oparte na ryzyku koncentruje zasoby na krytycznych częściach systemu."
                },
                {
                    "pytanie": "Jakie wyzwania niesie testowanie aplikacji mobilnych?",
                    "choices": {
                        "a": "Duża różnorodność urządzeń i systemów operacyjnych.",
                        "b": "Brak interfejsu użytkownika.",
                        "c": "Łatwość testowania.",
                        "d": "Brak potrzeby testowania."
                    },
                    "poprawna": "a",
                    "explanation": "Aplikacje mobilne muszą być testowane na wielu urządzeniach i wersjach systemów."
                },
                {
                    "pytanie": "Co to jest Continuous Testing?",
                    "choices": {
                        "a": "Testowanie wykonywane tylko na końcu projektu.",
                        "b": "Ciągłe uruchamianie testów podczas cyklu rozwoju oprogramowania.",
                        "c": "Wyłącznie testowanie manualne.",
                        "d": "Testowanie statyczne."
                    },
                    "poprawna": "b",
                    "explanation": "Continuous Testing oznacza regularne testowanie kodu na każdym etapie rozwoju."
                },
                {
                    "pytanie": "Jaki jest główny cel testów integracyjnych?",
                    "choices": {
                        "a": "Wykrycie błędów na styku modułów.",
                        "b": "Zwiększenie kosztów projektu.",
                        "c": "Opóźnienie wdrożenia.",
                        "d": "Testowanie interfejsu użytkownika."
                    },
                    "poprawna": "a",
                    "explanation": "Testy integracyjne identyfikują błędy powstające podczas współpracy modułów."
                },
                {
                    "pytanie": "Dlaczego ważne jest utrzymanie testów regresyjnych?",
                    "choices": {
                        "a": "Aby mieć pewność, że nowe zmiany nie psują istniejącej funkcjonalności.",
                        "b": "Ponieważ są bardzo szybkie.",
                        "c": "Testy regresyjne nie są istotne.",
                        "d": "Utrzymanie ich jest kosztowne."
                    },
                    "poprawna": "a",
                    "explanation": "Testy regresyjne pomagają zapewnić stabilność systemu po każdej modyfikacji."
                }
            ],
            "hard": [
                {
                    "pytanie": "Jakie wyzwania niesie testowanie aplikacji rozproszonych?",
                    "choices": {
                        "a": "Prosta konfiguracja.",
                        "b": "Synchronizacja danych i opóźnienia sieci.",
                        "c": "Brak potrzebnych narzędzi.",
                        "d": "Testowanie manualne wystarcza."
                    },
                    "poprawna": "b",
                    "explanation": "Testowanie rozproszonych aplikacji wymaga weryfikacji synchronizacji danych oraz radzenia sobie z opóźnieniami sieci."
                },
                {
                    "pytanie": "Czym jest testowanie A/B?",
                    "choices": {
                        "a": "Porównywanie dwóch wersji aplikacji.",
                        "b": "Testowanie bezpieczeństwa.",
                        "c": "Testowanie interfejsu.",
                        "d": "Testowanie integracyjne."
                    },
                    "poprawna": "a",
                    "explanation": "Testowanie A/B polega na porównaniu dwóch wariantów, aby wyłonić lepszą wersję."
                },
                {
                    "pytanie": "Jakie metryki są kluczowe w testach wydajnościowych?",
                    "choices": {
                        "a": "Czas odpowiedzi, przepustowość i obciążenie.",
                        "b": "Kolor interfejsu.",
                        "c": "Liczba znalezionych błędów.",
                        "d": "Koszt projektu."
                    },
                    "poprawna": "a",
                    "explanation": "Czas odpowiedzi, przepustowość oraz obciążenie to podstawowe miary wydajności systemu."
                },
                {
                    "pytanie": "Co to jest mocking w testach jednostkowych?",
                    "choices": {
                        "a": "Symulacja zależności, aby przetestować pojedynczą jednostkę.",
                        "b": "Testy integracyjne.",
                        "c": "Testowanie interfejsu.",
                        "d": "Testy wydajnościowe."
                    },
                    "poprawna": "a",
                    "explanation": "Mocking pozwala na symulowanie zachowania zależności, aby testować jednostkę w izolacji."
                },
                {
                    "pytanie": "Jakie są zalety stosowania frameworków testowych?",
                    "choices": {
                        "a": "Standaryzacja i ułatwienie pisania testów.",
                        "b": "Zwiększenie kosztów.",
                        "c": "Brak wsparcia społeczności.",
                        "d": "Trudniejsze testy."
                    },
                    "poprawna": "a",
                    "explanation": "Frameworki pomagają ujednolicić i usprawnić proces tworzenia testów."
                },
                {
                    "pytanie": "Czym jest testowanie oparte na modelu?",
                    "choices": {
                        "a": "Generowanie przypadków testowych na podstawie modelu matematycznego.",
                        "b": "Testowanie oparte na intuicji.",
                        "c": "Testowanie oparte na analizie ryzyka.",
                        "d": "Testowanie skryptowe."
                    },
                    "poprawna": "a",
                    "explanation": "Testowanie oparte na modelu wykorzystuje modele do automatycznego generowania przypadków testowych."
                },
                {
                    "pytanie": "Jak Continuous Integration wpływa na jakość oprogramowania?",
                    "choices": {
                        "a": "Pozwala na szybsze wykrywanie błędów.",
                        "b": "Zwiększa ryzyko błędów.",
                        "c": "Nie ma wpływu na jakość.",
                        "d": "Utrudnia wdrożenie."
                    },
                    "poprawna": "a",
                    "explanation": "CI umożliwia częste testowanie, co skutkuje wcześniejszym wykrywaniem problemów."
                },
                {
                    "pytanie": "Jakie wyzwania wiążą się z testowaniem systemów czasu rzeczywistego?",
                    "choices": {
                        "a": "Brak określonych terminów.",
                        "b": "Wymagana wysoka precyzja testów.",
                        "c": "Tests wymagają minimalnej synchronizacji.",
                        "d": "Łatwe wykrywanie błędów."
                    },
                    "poprawna": "b",
                    "explanation": "Systemy czasu rzeczywistego wymagają precyzyjnego testowania terminowości."
                },
                {
                    "pytanie": "Co to jest strategia testowania ryzykowego?",
                    "choices": {
                        "a": "Planowanie testów w oparciu o potencjalne ryzyka.",
                        "b": "Równomierne testowanie wszystkich funkcji.",
                        "c": "Testowanie oparte na analizie pokrycia kodu.",
                        "d": "Testowanie wyłącznie ręczne."
                    },
                    "poprawna": "a",
                    "explanation": "Strategia ryzykowa koncentruje testy na obszarach o największym ryzyku awarii."
                },
                {
                    "pytanie": "Jakie korzyści daje stosowanie testów end-to-end?",
                    "choices": {
                        "a": "Weryfikację całego przepływu użytkownika przez system.",
                        "b": "Testowanie pojedynczych funkcji.",
                        "c": "Testy wydajnościowe.",
                        "d": "Brak realnych korzyści."
                    },
                    "poprawna": "a",
                    "explanation": "Testy end-to-end sprawdzają kompletną ścieżkę użytkownika, gwarantując spójność systemu."
                }
            ]
        },
        "en": {
            "easy": [
                {
                    "question": "What is software testing?",
                    "choices": {
                        "a": "Writing code.",
                        "b": "Checking software.",
                        "c": "Creating documentation.",
                        "d": "Optimizing hardware."
                    },
                    "correct": "b",
                    "explanation": "Software testing verifies that the software functions as expected."
                },
                {
                    "question": "What are unit tests?",
                    "choices": {
                        "a": "Testing the entire system.",
                        "b": "Testing individual functions or modules.",
                        "c": "UI tests.",
                        "d": "Performance tests."
                    },
                    "correct": "b",
                    "explanation": "Unit tests focus on individual components of the software."
                },
                {
                    "question": "What is automated testing?",
                    "choices": {
                        "a": "Manual testing.",
                        "b": "Testing using tools.",
                        "c": "Testing using static analysis.",
                        "d": "Testing using real-time monitoring."
                    },
                    "correct": "b",
                    "explanation": "Automated testing uses tools to execute tests automatically."
                },
                {
                    "question": "What does regression testing involve?",
                    "choices": {
                        "a": "Testing new features.",
                        "b": "Retesting after code changes.",
                        "c": "Interface testing.",
                        "d": "Load testing."
                    },
                    "correct": "b",
                    "explanation": "Regression testing ensures recent changes haven't broken existing functionality."
                },
                {
                    "question": "What are integration tests?",
                    "choices": {
                        "a": "Tests for module interactions.",
                        "b": "UI tests.",
                        "c": "Security tests.",
                        "d": "Performance tests."
                    },
                    "correct": "a",
                    "explanation": "Integration tests check if different modules work together correctly."
                },
                {
                    "question": "What is exploratory testing?",
                    "choices": {
                        "a": "Scripted testing.",
                        "b": "Unscripted testing to discover bugs.",
                        "c": "Performance testing.",
                        "d": "Regression testing."
                    },
                    "correct": "b",
                    "explanation": "Exploratory testing is performed without predefined test cases."
                },
                {
                    "question": "What is manual testing?",
                    "choices": {
                        "a": "Testing using tools.",
                        "b": "Testing performed by humans.",
                        "c": "Automated testing.",
                        "d": "Integration testing."
                    },
                    "correct": "b",
                    "explanation": "Manual testing is conducted by human testers."
                },
                {
                    "question": "What is a bug in software?",
                    "choices": {
                        "a": "A new feature.",
                        "b": "An error in the software.",
                        "c": "A piece of code.",
                        "d": "A test case."
                    },
                    "correct": "b",
                    "explanation": "A bug is a defect in the software."
                },
                {
                    "question": "Why is test documentation important?",
                    "choices": {
                        "a": "It helps in repeating tests.",
                        "b": "It speeds up coding.",
                        "c": "It is not important.",
                        "d": "It increases errors."
                    },
                    "correct": "a",
                    "explanation": "Documentation ensures tests can be repeated and analyzed."
                },
                {
                    "question": "What is a test case?",
                    "choices": {
                        "a": "A scenario to test a function.",
                        "b": "A bug report.",
                        "c": "A piece of code.",
                        "d": "A documentation element."
                    },
                    "correct": "a",
                    "explanation": "A test case describes a specific scenario to be tested."
                }
            ],
            "medium": [
                {
                    "question": "What is regression testing?",
                    "choices": {
                        "a": "Testing new features.",
                        "b": "Retesting after code changes.",
                        "c": "Performance testing.",
                        "d": "UI testing."
                    },
                    "correct": "b",
                    "explanation": "Regression testing ensures that changes do not break existing functionality."
                },
                {
                    "question": "What are the benefits of test automation?",
                    "choices": {
                        "a": "Increased repeatability of tests.",
                        "b": "Higher costs.",
                        "c": "More manual effort required.",
                        "d": "Complex setup."
                    },
                    "correct": "a",
                    "explanation": "Automation increases test repeatability and efficiency."
                },
                {
                    "question": "What are load tests?",
                    "choices": {
                        "a": "Tests that evaluate system performance under heavy usage.",
                        "b": "UI tests.",
                        "c": "Regression tests.",
                        "d": "Security tests."
                    },
                    "correct": "a",
                    "explanation": "Load tests measure how the system performs under high traffic."
                },
                {
                    "question": "Which tool is popular for automated testing?",
                    "choices": {
                        "a": "Selenium",
                        "b": "Photoshop",
                        "c": "Microsoft Word",
                        "d": "Excel"
                    },
                    "correct": "a",
                    "explanation": "Selenium is widely used for web application testing."
                },
                {
                    "question": "What does CI/CD stand for?",
                    "choices": {
                        "a": "Continuous Integration/Continuous Deployment",
                        "b": "Central Integration/Continuous Development",
                        "c": "Continuous Inspection/Continuous Documentation",
                        "d": "Critical Integration/Critical Deployment"
                    },
                    "correct": "a",
                    "explanation": "CI/CD refers to practices that enable continuous integration and delivery."
                },
                {
                    "question": "What is risk-based testing?",
                    "choices": {
                        "a": "Testing every function equally.",
                        "b": "Focusing on high-risk areas.",
                        "c": "Testing based on code coverage analysis.",
                        "d": "UI testing."
                    },
                    "correct": "b",
                    "explanation": "Risk-based testing prioritizes testing of critical parts of the application."
                },
                {
                    "question": "What challenges do mobile applications present?",
                    "choices": {
                        "a": "Device and OS fragmentation.",
                        "b": "Lack of user interface.",
                        "c": "Easier testing.",
                        "d": "No testing required."
                    },
                    "correct": "a",
                    "explanation": "Mobile testing is challenging due to the variety of devices and operating systems."
                },
                {
                    "question": "What is Continuous Testing?",
                    "choices": {
                        "a": "Testing only at the end of development.",
                        "b": "Regularly running tests throughout development.",
                        "c": "Manual testing only.",
                        "d": "Static testing."
                    },
                    "correct": "b",
                    "explanation": "Continuous Testing involves running tests continuously during the development lifecycle."
                },
                {
                    "question": "What is the main benefit of integration testing?",
                    "choices": {
                        "a": "Detecting errors at module boundaries.",
                        "b": "Increasing project costs.",
                        "c": "Delaying deployment.",
                        "d": "Testing the UI only."
                    },
                    "correct": "a",
                    "explanation": "Integration tests help uncover issues at the interaction points between modules."
                },
                {
                    "question": "Why is maintaining regression tests important?",
                    "choices": {
                        "a": "To ensure that new changes do not break existing functionality.",
                        "b": "Because they are fast.",
                        "c": "They are not important.",
                        "d": "They reduce costs."
                    },
                    "correct": "a",
                    "explanation": "Regression tests provide confidence that system stability is maintained after changes."
                }
            ],
            "hard": [
                {
                    "question": "What challenges does testing distributed applications pose?",
                    "choices": {
                        "a": "Simple configuration.",
                        "b": "Data synchronization and network latency.",
                        "c": "Lack of necessary tools.",
                        "d": "Manual testing is sufficient."
                    },
                    "correct": "b",
                    "explanation": "Distributed applications require handling data consistency and network delays."
                },
                {
                    "question": "What is A/B testing?",
                    "choices": {
                        "a": "Comparing two versions of an application.",
                        "b": "Security testing.",
                        "c": "Integration testing.",
                        "d": "Load testing."
                    },
                    "correct": "a",
                    "explanation": "A/B testing compares two variants to determine which performs better."
                },
                {
                    "question": "Which metrics are crucial in performance testing?",
                    "choices": {
                        "a": "Response time, throughput, and load.",
                        "b": "UI design.",
                        "c": "Number of bugs.",
                        "d": "Project cost."
                    },
                    "correct": "a",
                    "explanation": "Key performance metrics include response time, throughput, and load capacity."
                },
                {
                    "question": "What is mocking in unit tests?",
                    "choices": {
                        "a": "Simulating dependencies to test a unit.",
                        "b": "Integration testing.",
                        "c": "UI testing.",
                        "d": "Performance testing."
                    },
                    "correct": "a",
                    "explanation": "Mocking isolates the unit under test by simulating external dependencies."
                },
                {
                    "question": "What are the advantages of using test frameworks?",
                    "choices": {
                        "a": "Standardizing tests and making them easier to write.",
                        "b": "Increasing costs.",
                        "c": "Less community support.",
                        "d": "More complex tests."
                    },
                    "correct": "a",
                    "explanation": "Test frameworks streamline test development and ensure consistency."
                },
                {
                    "question": "What is model-based testing?",
                    "choices": {
                        "a": "Generating test cases based on a mathematical model.",
                        "b": "Testing based on intuition.",
                        "c": "Risk-based testing.",
                        "d": "Scripted testing."
                    },
                    "correct": "a",
                    "explanation": "Model-based testing uses models to generate test cases automatically."
                },
                {
                    "question": "How does Continuous Integration affect software quality?",
                    "choices": {
                        "a": "It enables faster bug detection.",
                        "b": "It increases bug risk.",
                        "c": "It has no impact.",
                        "d": "It complicates deployment."
                    },
                    "correct": "a",
                    "explanation": "Continuous Integration allows frequent testing and early bug detection."
                },
                {
                    "question": "What challenges are associated with testing real-time systems?",
                    "choices": {
                        "a": "Lack of timing constraints.",
                        "b": "High precision required in tests.",
                        "c": "Tests do not require synchronization.",
                        "d": "Easy bug detection."
                    },
                    "correct": "b",
                    "explanation": "Real-time systems demand precise tests to verify strict timing requirements."
                },
                {
                    "question": "What is a risk-based testing strategy?",
                    "choices": {
                        "a": "Planning tests based on potential risks.",
                        "b": "Testing all features evenly.",
                        "c": "No test planning.",
                        "d": "Only manual testing."
                    },
                    "correct": "a",
                    "explanation": "Risk-based testing focuses resources on areas with the highest risk of failure."
                },
                {
                    "question": "What are the benefits of end-to-end testing?",
                    "choices": {
                        "a": "Verifying the entire user journey.",
                        "b": "Testing individual functions.",
                        "c": "Only performance tests.",
                        "d": "No real benefits."
                    },
                    "correct": "a",
                    "explanation": "End-to-end tests validate the complete flow of an application."
                }
            ]
        },
        "de": {
            "easy": [
                {
                    "frage": "Was ist Softwaretest?",
                    "choices": {
                        "a": "Code schreiben.",
                        "b": "Software überprüfen.",
                        "c": "Dokumentation erstellen.",
                        "d": "Hardware optimieren."
                    },
                    "korrekt": "b",
                    "erklärung": "Softwaretests überprüfen, ob die Software wie erwartet funktioniert."
                },
                {
                    "frage": "Was sind Unit-Tests?",
                    "choices": {
                        "a": "Testen des gesamten Systems.",
                        "b": "Testen einzelner Funktionen oder Module.",
                        "c": "UI-Tests.",
                        "d": "Leistungstests."
                    },
                    "korrekt": "b",
                    "erklärung": "Unit-Tests konzentrieren sich auf einzelne Softwarekomponenten."
                },
                {
                    "frage": "Was ist automatisiertes Testen?",
                    "choices": {
                        "a": "Manuelles Testen.",
                        "b": "Testen mit Werkzeugen.",
                        "c": "Testen mittels statischer Codeanalyse.",
                        "d": "Testen mittels Echtzeitüberwachung."
                    },
                    "korrekt": "b",
                    "erklärung": "Automatisiertes Testen verwendet Werkzeuge, um Tests automatisch auszuführen."
                },
                {
                    "frage": "Was bedeutet Regressionstest?",
                    "choices": {
                        "a": "Testen neuer Funktionen.",
                        "b": "Wiederholtes Testen nach Änderungen.",
                        "c": "UI-Test.",
                        "d": "Leistungstest."
                    },
                    "korrekt": "b",
                    "erklärung": "Regressionstests stellen sicher, dass Änderungen bestehende Funktionen nicht beeinträchtigen."
                },
                {
                    "frage": "Was sind Integrationstests?",
                    "choices": {
                        "a": "Tests der Modul-Interaktionen.",
                        "b": "UI-Tests.",
                        "c": "Sicherheitstests.",
                        "d": "Leistungstests."
                    },
                    "korrekt": "a",
                    "erklärung": "Integrationstests überprüfen, ob verschiedene Module korrekt zusammenarbeiten."
                },
                {
                    "frage": "Was versteht man unter explorativem Testen?",
                    "choices": {
                        "a": "Skriptbasiertes Testen.",
                        "b": "Unstrukturierte Tests zur Fehlerfindung.",
                        "c": "Leistungstest.",
                        "d": "Regressionstest."
                    },
                    "korrekt": "b",
                    "erklärung": "Exploratives Testen wird ohne vorgegebene Testfälle durchgeführt, um Fehler zu entdecken."
                },
                {
                    "frage": "Was ist manuelles Testen?",
                    "choices": {
                        "a": "Testen mit Werkzeugen.",
                        "b": "Testen durch Menschen.",
                        "c": "Automatisiertes Testen.",
                        "d": "Regressionstest."
                    },
                    "korrekt": "b",
                    "erklärung": "Manuelles Testen wird von menschlichen Testern durchgeführt."
                },
                {
                    "frage": "Was ist ein Bug?",
                    "choices": {
                        "a": "Eine neue Funktion.",
                        "b": "Ein Fehler in der Software.",
                        "c": "Ein Codeabschnitt.",
                        "d": "Ein Testfall."
                    },
                    "korrekt": "b",
                    "erklärung": "Ein Bug ist ein Fehler oder eine Unstimmigkeit in der Software."
                },
                {
                    "frage": "Warum ist Testdokumentation wichtig?",
                    "choices": {
                        "a": "Sie hilft, Tests zu wiederholen.",
                        "b": "Sie beschleunigt das Codieren.",
                        "c": "Sie ist unwichtig.",
                        "d": "Sie erhöht die Fehlerzahl."
                    },
                    "korrekt": "a",
                    "erklärung": "Dokumentation ermöglicht konsistente und wiederholbare Tests."
                },
                {
                    "frage": "Was ist ein Testfall?",
                    "choices": {
                        "a": "Ein Szenario zur Überprüfung einer Funktion.",
                        "b": "Ein Fehlerbericht.",
                        "c": "Ein Codeabschnitt.",
                        "d": "Ein Dokumentationselement."
                    },
                    "korrekt": "a",
                    "erklärung": "Ein Testfall beschreibt ein Szenario, das getestet werden soll."
                }
            ],
            "medium": [
                {
                    "frage": "Was bedeutet Regressionstesten?",
                    "choices": {
                        "a": "Testen neuer Funktionen.",
                        "b": "Wiederholtes Testen nach Änderungen.",
                        "c": "Leistungstesten.",
                        "d": "UI-Tests."
                    },
                    "korrekt": "b",
                    "erklärung": "Regressionstests überprüfen, ob nach Änderungen bestehende Funktionen weiterhin korrekt arbeiten."
                },
                {
                    "frage": "Welche Vorteile bietet automatisiertes Testen?",
                    "choices": {
                        "a": "Erhöhte Wiederholbarkeit der Tests.",
                        "b": "Höhere Kosten.",
                        "c": "Mehr manueller Aufwand.",
                        "d": "Komplexe Einrichtung."
                    },
                    "korrekt": "a",
                    "erklärung": "Automatisierung steigert die Wiederholbarkeit und Effizienz der Tests."
                },
                {
                    "frage": "Was sind Lasttests?",
                    "choices": {
                        "a": "Tests unter hoher Belastung.",
                        "b": "UI-Tests.",
                        "c": "Regressionstests.",
                        "d": "Sicherheitstests."
                    },
                    "korrekt": "a",
                    "erklärung": "Lasttests messen, wie das System bei hoher Nutzung reagiert."
                },
                {
                    "frage": "Welches Tool ist populär für automatisierte Tests?",
                    "choices": {
                        "a": "Selenium",
                        "b": "Photoshop",
                        "c": "Word",
                        "d": "Excel"
                    },
                    "korrekt": "a",
                    "erklärung": "Selenium ist weit verbreitet im Web-Testbereich."
                },
                {
                    "frage": "Wofür steht CI/CD?",
                    "choices": {
                        "a": "Continuous Integration/Continuous Deployment",
                        "b": "Central Integration/Continuous Development",
                        "c": "Continuous Inspection/Continuous Documentation",
                        "d": "Critical Integration/Critical Deployment"
                    },
                    "korrekt": "a",
                    "erklärung": "CI/CD bezeichnet Prozesse der kontinuierlichen Integration und Auslieferung."
                },
                {
                    "frage": "Was ist risikobasiertes Testen?",
                    "choices": {
                        "a": "Gleichmäßiges Testen aller Funktionen.",
                        "b": "Fokussierung auf risikoreiche Bereiche.",
                        "c": "Testen basierend auf Codeabdeckungsanalyse.",
                        "d": "UI-Tests."
                    },
                    "korrekt": "b",
                    "erklärung": "Risikobasiertes Testen konzentriert sich auf die kritischsten Systembereiche."
                },
                {
                    "frage": "Welche Herausforderungen stellen mobile Anwendungen im Testen dar?",
                    "choices": {
                        "a": "Gerätevielfalt und unterschiedliche Betriebssysteme.",
                        "b": "Fehlender UI.",
                        "c": "Einfacheres Testen.",
                        "d": "Kein Testbedarf."
                    },
                    "korrekt": "a",
                    "erklärung": "Die Vielfalt an Geräten und OS-Versionen macht mobile Tests anspruchsvoll."
                },
                {
                    "frage": "Was bedeutet Continuous Testing?",
                    "choices": {
                        "a": "Testen nur am Ende der Entwicklung.",
                        "b": "Kontinuierliches Testen während des gesamten Entwicklungsprozesses.",
                        "c": "Nur manuelles Testen.",
                        "d": "Statisches Testen."
                    },
                    "korrekt": "b",
                    "erklärung": "Continuous Testing sorgt für regelmäßige Überprüfung des Codes während der Entwicklung."
                },
                {
                    "frage": "Was ist der Nutzen von Integrationstests?",
                    "choices": {
                        "a": "Erkennen von Fehlern an den Schnittstellen zwischen Modulen.",
                        "b": "Erhöhte Kosten.",
                        "c": "Verzögerte Softwarebereitstellung.",
                        "d": "Kein wirklicher Nutzen."
                    },
                    "korrekt": "a",
                    "erklärung": "Integrationstests helfen, Fehler an den Übergängen zwischen Modulen zu identifizieren."
                },
                {
                    "frage": "Warum ist es wichtig, Regressionstests zu pflegen?",
                    "choices": {
                        "a": "Um sicherzustellen, dass Änderungen bestehende Funktionen nicht beeinträchtigen.",
                        "b": "Weil sie sehr schnell sind.",
                        "c": "Sie sind unwichtig.",
                        "d": "Weil sie die Kosten senken."
                    },
                    "korrekt": "a",
                    "erklärung": "Regressionstests gewährleisten, dass der bestehende Funktionsumfang erhalten bleibt."
                }
            ],
            "hard": [
                {
                    "frage": "Welche Herausforderungen gibt es beim Testen verteilter Anwendungen?",
                    "choices": {
                        "a": "Einfache Konfiguration.",
                        "b": "Datensynchronisation und Netzwerkverzögerungen.",
                        "c": "Keine notwendigen Werkzeuge.",
                        "d": "Manuelles Testen reicht aus."
                    },
                    "korrekt": "b",
                    "erklärung": "Verteilte Systeme erfordern Tests hinsichtlich Datenkonsistenz und Netzwerkverzögerungen."
                },
                {
                    "frage": "Was ist A/B-Testing?",
                    "choices": {
                        "a": "Vergleich zweier Versionen einer Anwendung.",
                        "b": "Sicherheitstests.",
                        "c": "Integrationstests.",
                        "d": "Lasttests."
                    },
                    "korrekt": "a",
                    "erklärung": "A/B-Testing vergleicht zwei Varianten, um die bessere Version zu ermitteln."
                },
                {
                    "frage": "Welche Metriken sind im Leistungstest entscheidend?",
                    "choices": {
                        "a": "Antwortzeit, Durchsatz und Belastung.",
                        "b": "Design der Benutzeroberfläche.",
                        "c": "Anzahl der gefundenen Fehler.",
                        "d": "Projektkosten."
                    },
                    "korrekt": "a",
                    "erklärung": "Wichtige Leistungsmetriken sind Antwortzeit, Durchsatz und Belastungsgrenzen."
                },
                {
                    "frage": "Was bedeutet Mocking in Unit-Tests?",
                    "choices": {
                        "a": "Simulation von Abhängigkeiten zur Isolation einer Testeinheit.",
                        "b": "Integrationstests.",
                        "c": "UI-Tests.",
                        "d": "Leistungstests."
                    },
                    "korrekt": "a",
                    "erklärung": "Mocking ermöglicht es, externe Abhängigkeiten zu simulieren, um den Test zu isolieren."
                },
                {
                    "frage": "Welche Vorteile bieten Test-Frameworks?",
                    "choices": {
                        "a": "Standardisierung und Erleichterung der Testentwicklung.",
                        "b": "Erhöhte Kosten.",
                        "c": "Weniger Community-Support.",
                        "d": "Komplexere Tests."
                    },
                    "korrekt": "a",
                    "erklärung": "Frameworks vereinfachen das Schreiben und Pflegen von Tests."
                },
                {
                    "frage": "Was versteht man unter modellbasiertem Testen?",
                    "choices": {
                        "a": "Testen anhand eines mathematischen Modells zur Generierung von Testfällen.",
                        "b": "Testen basierend auf Intuition.",
                        "c": "Risikobasiertes Testen.",
                        "d": "Scriptbasiertes Testen."
                    },
                    "korrekt": "a",
                    "erklärung": "Modellbasiertes Testen nutzt Modelle, um automatisch Testfälle zu erstellen."
                },
                {
                    "frage": "Wie wirkt sich Continuous Integration auf die Softwarequalität aus?",
                    "choices": {
                        "a": "Es ermöglicht eine schnellere Fehlererkennung.",
                        "b": "Es erhöht das Fehlerrisiko.",
                        "c": "Es hat keinen Einfluss.",
                        "d": "Es erschwert die Bereitstellung."
                    },
                    "korrekt": "a",
                    "erklärung": "Durch CI werden Änderungen häufig integriert und getestet, was die Fehlererkennung beschleunigt."
                },
                {
                    "frage": "Welche Herausforderungen bringt das Testen von Echtzeitsystemen mit sich?",
                    "choices": {
                        "a": "Fehlende Zeitvorgaben.",
                        "b": "Hohe Präzision in den Tests erforderlich.",
                        "c": "Tests erfordern keine Synchronisation.",
                        "d": "Einfaches Auffinden von Fehlern."
                    },
                    "korrekt": "b",
                    "erklärung": "Echtzeitsysteme erfordern sehr präzise Tests, um Zeitvorgaben einzuhalten."
                },
                {
                    "frage": "Was ist eine risikobasierte Teststrategie?",
                    "choices": {
                        "a": "Planung von Tests basierend auf potenziellen Risiken.",
                        "b": "Gleichmäßiges Testen aller Funktionen.",
                        "c": "Keine Testplanung.",
                        "d": "Nur manuelles Testen."
                    },
                    "korrekt": "a",
                    "erklärung": "Eine risikobasierte Strategie fokussiert sich auf Bereiche mit hohem Fehlerrisiko."
                },
                {
                    "frage": "Welche Vorteile bietet End-to-End-Testing?",
                    "choices": {
                        "a": "Überprüfung des gesamten Nutzerflusses.",
                        "b": "Testen einzelner Funktionen.",
                        "c": "Nur Leistungstests.",
                        "d": "Keine Vorteile."
                    },
                    "korrekt": "a",
                    "erklärung": "End-to-End-Tests validieren die komplette Anwendungskette und den Nutzerfluss."
                }
            ]
        }
    }

    # Słownik tłumaczeń interfejsu użytkownika – w tym komunikaty do trybu powtórki oraz komunikat końcowy
    ui_text = {
        "pl": {
            "question_label": "Pytanie",
            "choose_answer": "Wybierz odpowiedź (a, b, c, d): ",
            "correct": "Poprawna odpowiedź!",
            "incorrect": "Niepoprawna odpowiedź.",
            "correct_answer": "Prawidłowa odpowiedź to:",
            "explanation": "Wyjaśnienie:",
            "score": "Twój wynik:",
            "choose_difficulty": "Wybierz poziom trudności (łatwy/średni/trudny): ",
            "review_prompt": "Czy chcesz przejrzeć pytania, na które odpowiedziałeś niepoprawnie? (tak/nie): ",
            "review_header": "Przegląd pytań niepoprawnych:",
            "your_answer": "Twoja odpowiedź:",
            "final_message": "Dziękujemy za udział w quizie! Pomysłodawcą quizu jest Dominik Kurda."
        },
        "en": {
            "question_label": "Question",
            "choose_answer": "Choose an answer (a, b, c, d): ",
            "correct": "Correct answer!",
            "incorrect": "Incorrect answer.",
            "correct_answer": "Correct answer is:",
            "explanation": "Explanation:",
            "score": "Your score:",
            "choose_difficulty": "Choose difficulty level (easy/medium/hard): ",
            "review_prompt": "Would you like to review the questions you got wrong? (yes/no): ",
            "review_header": "Review of incorrect questions:",
            "your_answer": "Your answer:",
            "final_message": "Thank you for participating in the quiz! This quiz was inspired by an idea from Dominik Kurda."
        },
        "de": {
            "question_label": "Frage",
            "choose_answer": "Wähle eine Antwort (a, b, c, d): ",
            "correct": "Richtige Antwort!",
            "incorrect": "Falsche Antwort.",
            "correct_answer": "Die richtige Antwort ist:",
            "explanation": "Erklärung:",
            "score": "Dein Ergebnis:",
            "choose_difficulty": "Wähle den Schwierigkeitsgrad (einfach/mittel/schwer): ",
            "review_prompt": "Möchten Sie die falsch beantworteten Fragen überprüfen? (ja/nein): ",
            "review_header": "Überprüfung der falsch beantworteten Fragen:",
            "your_answer": "Ihre Antwort:",
            "final_message": "Vielen Dank für die Teilnahme am Quiz! Die Idee zu diesem Quiz stammt von Dominik Kurda."
        }
    }

    # Wybór języka
    lang = input("Wybierz język / Choose language / Wählen Sie die Sprache (pl/en/de): ").strip().lower()
    if lang not in quizzes:
        print("Niepoprawny wybór. Domyślnie ustawiono język polski.")
        lang = "pl"
    texts = ui_text[lang]

    # Wybór poziomu trudności
    diff = input(texts["choose_difficulty"]).strip().lower()
    valid_difficulties = {
        "pl": {"łatwy": "easy", "średni": "medium", "trudny": "hard"},
        "en": {"easy": "easy", "medium": "medium", "hard": "hard"},
        "de": {"einfach": "easy", "mittel": "medium", "schwer": "hard"}
    }
    if diff not in valid_difficulties[lang]:
        default_diff = list(valid_difficulties[lang].keys())[0]
        msg = ("Niepoprawny wybór. Domyślnie ustawiono poziom łatwy." if lang == "pl"
               else "Invalid choice. Defaulting to easy level." if lang == "en"
               else "Ungültige Auswahl. Standardmäßig wird 'einfach' gewählt.")
        print(msg)
        diff = default_diff
    chosen_diff = valid_difficulties[lang][diff]

    # Pobranie quizu dla wybranego języka i poziomu trudności oraz losowe przemieszanie pytań
    quiz = quizzes[lang][chosen_diff]
    random.shuffle(quiz)
    score = 0

    # Lista przechowująca pytania, na które udzielono niepoprawnej odpowiedzi
    wrong_questions = []

    # Ustalenie kluczy do pobierania treści pytania, poprawnej odpowiedzi i wyjaśnienia w zależności od języka
    if lang == "pl":
        question_key = "pytanie"
        correct_key = "poprawna"
        explanation_key = "explanation"
    elif lang == "en":
        question_key = "question"
        correct_key = "correct"
        explanation_key = "explanation"
    elif lang == "de":
        question_key = "frage"
        correct_key = "korrekt"
        explanation_key = "erklärung"

    # Pętla prezentująca pytania
    for i, item in enumerate(quiz, start=1):
        print(f"\n{texts['question_label']} {i}: {item[question_key]}")
        for key, value in item["choices"].items():
            print(f"{key}) {value}")
        user_answer = input(texts["choose_answer"]).strip().lower()
        if user_answer == item[correct_key]:
            print(texts["correct"])
            score += 1
        else:
            correct_option = item[correct_key]
            correct_text = item["choices"][correct_option]
            print(texts["incorrect"])
            print(f"{texts['correct_answer']} {correct_option}) {correct_text}")
            print(f"{texts['explanation']} {item[explanation_key]}")
            # Zapisz pytanie do listy pytań niepoprawnych z dodatkową informacją o udzielonej odpowiedzi
            entry = item.copy()
            entry["user_answer"] = user_answer
            wrong_questions.append(entry)

    print(f"\n{texts['score']} {score} na {len(quiz)}")

    # Tryb powtórki - przegląd pytań, na które odpowiedziałeś niepoprawnie
    if wrong_questions:
        review = input(texts["review_prompt"]).strip().lower()
        if review in ["tak", "yes", "ja"]:
            print(f"\n{texts['review_header']}")
            for idx, entry in enumerate(wrong_questions, start=1):
                print(f"\n{idx}. {entry[question_key]}")
                for key, value in entry["choices"].items():
                    print(f"{key}) {value}")
                print(f"{texts['your_answer']} {entry['user_answer']}")
                correct_opt = entry[correct_key]
                print(f"{texts['correct_answer']} {correct_opt}) {entry['choices'][correct_opt]}")
                print(f"{texts['explanation']} {entry[explanation_key]}")

    # Komunikat końcowy po trybie powtórki
    print("\n" + texts["final_message"])

if __name__ == '__main__':
    run_quiz()
