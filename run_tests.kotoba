(require '[clojure.test :as t])

(doseq [ns-sym '[suimin.methods.test-charter-gates
                  suimin.murakumo-test
                  suimin.repository-contract-test]]
  (require ns-sym))

(let [result (apply t/run-tests
                    '[suimin.methods.test-charter-gates
                      suimin.murakumo-test
                      suimin.repository-contract-test])]
  (System/exit (if (zero? (+ (:fail result) (:error result))) 0 1)))
