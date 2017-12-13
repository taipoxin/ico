Заметки:

solidity возвращает invalid opcode при require(false) в теле вызываемой функции

to call custom function and get result use:

    Contract.deployed().then(i => i.functionName.call(param1, param2))

example:

    ConvertLib.deployed().then(i => i.convert.call(100, 10))
    ICOBooster.deployed().then(i=> i.createCampaign.call())

not (without result, only json)

    ConvertLib.deployed().then(i=>i.convert(100, 10)).then(k=>k.value)





