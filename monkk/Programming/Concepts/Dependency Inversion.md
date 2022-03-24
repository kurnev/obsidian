Внедрение зависимости, внедряем зависимость прямо в компонент типо, как пример с логгером

class UserService {
..

constructior(_logger private: Logger) {}

}

const logger = new Logger();
const userService = new UserSerivce(logger); <- внедрение зависимости