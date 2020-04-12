## ansible-playbook playbook.yml -i inventory  -- > will do audit and remediat if the host is non complaint and revalidate the audit after remedation.

### Running the above play second time will only do audit and will not remediate since its already remediated.

## ansible-playbook playook.yml -i inventory -e 'remediate_own: true' --> it will remediate the files even audit is sucess and revalidate it.

## ansible-playbook playbook.yml -i inventory --tags "audit" --> it will only audit
