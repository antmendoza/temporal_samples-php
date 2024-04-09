- docker compose down --remove-orphans && docker volume prune -f

- docker compose build && docker compose up

- tctl workflow start --tq "default" --wt "Signal.greet" --workflow_id "my-php-signal"

- tctl workflow start --tq "default" --wt "SimpleActivity.greet" --workflow_id "my-php-signal"

- tctl workflow signal --workflow_id my-php-signal --name addName --input \"signal1\"

- stop docker compose ctrl+c

- docker compose up

- tctl workflow signal --workflow_id my-php-signal --name addName --input \"signal2\"
