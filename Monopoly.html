import React, { useState, useEffect } from 'react';
import { Users, DollarSign, Dices, Settings, Home, Building2, Landmark, Factory, Train, Zap, Droplet, HelpCircle } from 'lucide-react';

const MonopolyGame = () => {
  const [gameStarted, setGameStarted] = useState(false);
  const [numPlayers, setNumPlayers] = useState(2);
  const [startingMoney, setStartingMoney] = useState(1500);
  const [players, setPlayers] = useState([]);
  const [currentPlayerIndex, setCurrentPlayerIndex] = useState(0);
  const [dice1, setDice1] = useState(1);
  const [dice2, setDice2] = useState(1);
  const [doubles, setDoubles] = useState(0);
  const [message, setMessage] = useState('');
  const [showSettings, setShowSettings] = useState(false);

  const properties = [
    { id: 0, name: 'إبدأ', type: 'go', color: 'red' },
    { id: 1, name: 'شارع المدينة', type: 'property', price: 60, rent: [2, 10, 30, 90, 160, 250], color: 'brown', group: 1 },
    { id: 2, name: 'صندوق المجتمع', type: 'community', color: 'lightblue' },
    { id: 3, name: 'شارع الجامعة', type: 'property', price: 60, rent: [4, 20, 60, 180, 320, 450], color: 'brown', group: 1 },
    { id: 4, name: 'ضريبة الدخل', type: 'tax', amount: 200, color: 'pink' },
    { id: 5, name: 'محطة القطار 1', type: 'station', price: 200, rent: [25, 50, 100, 200], color: 'gray' },
    { id: 6, name: 'شارع النور', type: 'property', price: 100, rent: [6, 30, 90, 270, 400, 550], color: 'lightblue', group: 2 },
    { id: 7, name: 'فرصة', type: 'chance', color: 'orange' },
    { id: 8, name: 'شارع السلام', type: 'property', price: 100, rent: [6, 30, 90, 270, 400, 550], color: 'lightblue', group: 2 },
    { id: 9, name: 'شارع الحرية', type: 'property', price: 120, rent: [8, 40, 100, 300, 450, 600], color: 'lightblue', group: 2 },
    { id: 10, name: 'السجن', type: 'jail', color: 'orange' },
    { id: 11, name: 'شارع الأمل', type: 'property', price: 140, rent: [10, 50, 150, 450, 625, 750], color: 'purple', group: 3 },
    { id: 12, name: 'شركة الكهرباء', type: 'utility', price: 150, color: 'yellow' },
    { id: 13, name: 'شارع النصر', type: 'property', price: 140, rent: [10, 50, 150, 450, 625, 750], color: 'purple', group: 3 },
    { id: 14, name: 'شارع التقدم', type: 'property', price: 160, rent: [12, 60, 180, 500, 700, 900], color: 'purple', group: 3 },
    { id: 15, name: 'محطة القطار 2', type: 'station', price: 200, rent: [25, 50, 100, 200], color: 'gray' },
    { id: 16, name: 'شارع الوحدة', type: 'property', price: 180, rent: [14, 70, 200, 550, 750, 950], color: 'orange', group: 4 },
    { id: 17, name: 'صندوق المجتمع', type: 'community', color: 'lightblue' },
    { id: 18, name: 'شارع العروبة', type: 'property', price: 180, rent: [14, 70, 200, 550, 750, 950], color: 'orange', group: 4 },
    { id: 19, name: 'شارع الاستقلال', type: 'property', price: 200, rent: [16, 80, 220, 600, 800, 1000], color: 'orange', group: 4 },
    { id: 20, name: 'موقف مجاني', type: 'parking', color: 'red' },
    { id: 21, name: 'شارع النهضة', type: 'property', price: 220, rent: [18, 90, 250, 700, 875, 1050], color: 'red', group: 5 },
    { id: 22, name: 'فرصة', type: 'chance', color: 'orange' },
    { id: 23, name: 'شارع البناء', type: 'property', price: 220, rent: [18, 90, 250, 700, 875, 1050], color: 'red', group: 5 },
    { id: 24, name: 'شارع التنمية', type: 'property', price: 240, rent: [20, 100, 300, 750, 925, 1100], color: 'red', group: 5 },
    { id: 25, name: 'محطة القطار 3', type: 'station', price: 200, rent: [25, 50, 100, 200], color: 'gray' },
    { id: 26, name: 'شارع الازدهار', type: 'property', price: 260, rent: [22, 110, 330, 800, 975, 1150], color: 'yellow', group: 6 },
    { id: 27, name: 'شارع الرخاء', type: 'property', price: 260, rent: [22, 110, 330, 800, 975, 1150], color: 'yellow', group: 6 },
    { id: 28, name: 'شركة المياه', type: 'utility', price: 150, color: 'yellow' },
    { id: 29, name: 'شارع السعادة', type: 'property', price: 280, rent: [24, 120, 360, 850, 1025, 1200], color: 'yellow', group: 6 },
    { id: 30, name: 'اذهب للسجن', type: 'gotojail', color: 'red' },
    { id: 31, name: 'شارع الفخامة', type: 'property', price: 300, rent: [26, 130, 390, 900, 1100, 1275], color: 'green', group: 7 },
    { id: 32, name: 'شارع الرقي', type: 'property', price: 300, rent: [26, 130, 390, 900, 1100, 1275], color: 'green', group: 7 },
    { id: 33, name: 'صندوق المجتمع', type: 'community', color: 'lightblue' },
    { id: 34, name: 'شارع الثروة', type: 'property', price: 320, rent: [28, 150, 450, 1000, 1200, 1400], color: 'green', group: 7 },
    { id: 35, name: 'محطة القطار 4', type: 'station', price: 200, rent: [25, 50, 100, 200], color: 'gray' },
    { id: 36, name: 'فرصة', type: 'chance', color: 'orange' },
    { id: 37, name: 'شارع الماس', type: 'property', price: 350, rent: [35, 175, 500, 1100, 1300, 1500], color: 'blue', group: 8 },
    { id: 38, name: 'ضريبة الترف', type: 'tax', amount: 100, color: 'pink' },
    { id: 39, name: 'شارع الذهب', type: 'property', price: 400, rent: [50, 200, 600, 1400, 1700, 2000], color: 'blue', group: 8 }
  ];

  const playerColors = ['#e74c3c', '#3498db', '#2ecc71', '#f39c12'];
  const playerNames = ['اللاعب 1', 'اللاعب 2', 'اللاعب 3', 'اللاعب 4'];

  const initGame = () => {
    const newPlayers = [];
    for (let i = 0; i < numPlayers; i++) {
      newPlayers.push({
        id: i,
        name: playerNames[i],
        money: startingMoney,
        position: 0,
        properties: [],
        inJail: false,
        jailTurns: 0,
        color: playerColors[i],
        bankrupt: false
      });
    }
    setPlayers(newPlayers);
    setCurrentPlayerIndex(0);
    setGameStarted(true);
    setMessage(`${playerNames[0]} - دورك!`);
  };

  const rollDice = () => {
    if (players[currentPlayerIndex].bankrupt) {
      nextPlayer();
      return;
    }

    const d1 = Math.floor(Math.random() * 6) + 1;
    const d2 = Math.floor(Math.random() * 6) + 1;
    setDice1(d1);
    setDice2(d2);

    const currentPlayer = players[currentPlayerIndex];
    
    if (currentPlayer.inJail) {
      if (d1 === d2) {
        const updated = [...players];
        updated[currentPlayerIndex].inJail = false;
        updated[currentPlayerIndex].jailTurns = 0;
        setPlayers(updated);
        movePlayer(d1 + d2);
        setMessage(`${currentPlayer.name} خرج من السجن بالنرد المتطابق!`);
      } else {
        const updated = [...players];
        updated[currentPlayerIndex].jailTurns++;
        if (updated[currentPlayerIndex].jailTurns >= 3) {
          updated[currentPlayerIndex].money -= 50;
          updated[currentPlayerIndex].inJail = false;
          updated[currentPlayerIndex].jailTurns = 0;
          setMessage(`${currentPlayer.name} دفع 50$ للخروج من السجن`);
        } else {
          setMessage(`${currentPlayer.name} لا يزال في السجن`);
        }
        setPlayers(updated);
        setTimeout(nextPlayer, 2000);
      }
      return;
    }

    if (d1 === d2) {
      setDoubles(doubles + 1);
      if (doubles + 1 >= 3) {
        sendToJail();
        return;
      }
    } else {
      setDoubles(0);
    }

    movePlayer(d1 + d2);
  };

  const movePlayer = (steps) => {
    const updated = [...players];
    const oldPos = updated[currentPlayerIndex].position;
    let newPos = (oldPos + steps) % 40;
    
    if (newPos < oldPos) {
      updated[currentPlayerIndex].money += 200;
      setMessage(`${updated[currentPlayerIndex].name} مر من البداية وحصل على 200$!`);
    }
    
    updated[currentPlayerIndex].position = newPos;
    setPlayers(updated);
    
    setTimeout(() => {
      handleLanding(newPos);
    }, 500);
  };

  const handleLanding = (position) => {
    const property = properties[position];
    const currentPlayer = players[currentPlayerIndex];
    
    switch(property.type) {
      case 'go':
        setMessage(`${currentPlayer.name} على البداية!`);
        setTimeout(() => {
          if (dice1 !== dice2) nextPlayer();
          else setMessage(`${currentPlayer.name} - العب مرة أخرى!`);
        }, 2000);
        break;
        
      case 'property':
      case 'station':
      case 'utility':
        handlePropertyLanding(property);
        break;
        
      case 'tax':
        payTax(property.amount);
        break;
        
      case 'gotojail':
        sendToJail();
        break;
        
      case 'jail':
        setMessage(`${currentPlayer.name} في زيارة للسجن فقط`);
        setTimeout(() => {
          if (dice1 !== dice2) nextPlayer();
          else setMessage(`${currentPlayer.name} - العب مرة أخرى!`);
        }, 2000);
        break;
        
      case 'parking':
        setMessage(`${currentPlayer.name} في موقف مجاني!`);
        setTimeout(() => {
          if (dice1 !== dice2) nextPlayer();
          else setMessage(`${currentPlayer.name} - العب مرة أخرى!`);
        }, 2000);
        break;
        
      case 'chance':
      case 'community':
        handleCard(property.type);
        break;
        
      default:
        setTimeout(() => {
          if (dice1 !== dice2) nextPlayer();
          else setMessage(`${currentPlayer.name} - العب مرة أخرى!`);
        }, 2000);
    }
  };

  const handlePropertyLanding = (property) => {
    const currentPlayer = players[currentPlayerIndex];
    const owner = players.find(p => p.properties.includes(property.id));
    
    if (!owner) {
      setMessage(`${currentPlayer.name} على ${property.name} - السعر ${property.price}$ (اضغط شراء)`);
    } else if (owner.id === currentPlayer.id) {
      setMessage(`${currentPlayer.name} على ممتلكاته - ${property.name}`);
      setTimeout(() => {
        if (dice1 !== dice2) nextPlayer();
        else setMessage(`${currentPlayer.name} - العب مرة أخرى!`);
      }, 2000);
    } else {
      const rent = calculateRent(property, owner);
      payRent(owner, rent);
    }
  };

  const calculateRent = (property, owner) => {
    if (property.type === 'station') {
      const stationsOwned = properties.filter(p => 
        p.type === 'station' && owner.properties.includes(p.id)
      ).length;
      return property.rent[stationsOwned - 1];
    } else if (property.type === 'utility') {
      const utilitiesOwned = properties.filter(p => 
        p.type === 'utility' && owner.properties.includes(p.id)
      ).length;
      return utilitiesOwned === 2 ? (dice1 + dice2) * 10 : (dice1 + dice2) * 4;
    } else {
      return property.rent[0];
    }
  };

  const buyProperty = () => {
    const property = properties[players[currentPlayerIndex].position];
    if (property.type !== 'property' && property.type !== 'station' && property.type !== 'utility') return;
    
    const owner = players.find(p => p.properties.includes(property.id));
    if (owner) return;
    
    const updated = [...players];
    if (updated[currentPlayerIndex].money >= property.price) {
      updated[currentPlayerIndex].money -= property.price;
      updated[currentPlayerIndex].properties.push(property.id);
      setPlayers(updated);
      setMessage(`${updated[currentPlayerIndex].name} اشترى ${property.name}!`);
      setTimeout(() => {
        if (dice1 !== dice2) nextPlayer();
        else setMessage(`${updated[currentPlayerIndex].name} - العب مرة أخرى!`);
      }, 2000);
    } else {
      setMessage(`${updated[currentPlayerIndex].name} ليس لديه مال كافٍ!`);
    }
  };

  const payRent = (owner, amount) => {
    const updated = [...players];
    updated[currentPlayerIndex].money -= amount;
    updated[owner.id].money += amount;
    
    if (updated[currentPlayerIndex].money < 0) {
      updated[currentPlayerIndex].bankrupt = true;
      setMessage(`${updated[currentPlayerIndex].name} مفلس! دفع ${amount}$ لـ ${owner.name}`);
    } else {
      setMessage(`${updated[currentPlayerIndex].name} دفع ${amount}$ إيجار لـ ${owner.name}`);
    }
    
    setPlayers(updated);
    setTimeout(() => {
      if (dice1 !== dice2) nextPlayer();
      else setMessage(`${updated[currentPlayerIndex].name} - العب مرة أخرى!`);
    }, 2000);
  };

  const payTax = (amount) => {
    const updated = [...players];
    updated[currentPlayerIndex].money -= amount;
    
    if (updated[currentPlayerIndex].money < 0) {
      updated[currentPlayerIndex].bankrupt = true;
    }
    
    setPlayers(updated);
    setMessage(`${updated[currentPlayerIndex].name} دفع ${amount}$ ضريبة`);
    setTimeout(() => {
      if (dice1 !== dice2) nextPlayer();
      else setMessage(`${updated[currentPlayerIndex].name} - العب مرة أخرى!`);
    }, 2000);
  };

  const sendToJail = () => {
    const updated = [...players];
    updated[currentPlayerIndex].position = 10;
    updated[currentPlayerIndex].inJail = true;
    updated[currentPlayerIndex].jailTurns = 0;
    setPlayers(updated);
    setMessage(`${updated[currentPlayerIndex].name} ذهب للسجن!`);
    setDoubles(0);
    setTimeout(nextPlayer, 2000);
  };

  const handleCard = (type) => {
    const cards = type === 'chance' ? [
      'تقدم للبداية واحصل على 200$',
      'ارجع 3 خطوات',
      'اذهب للسجن',
      'احصل على 50$',
      'ادفع 15$ للبنك'
    ] : [
      'احصل على 100$',
      'ادفع 50$ للمستشفى',
      'اخرج من السجن مجاناً',
      'تقدم للبداية',
      'احصل على 25$'
    ];
    
    const card = cards[Math.floor(Math.random() * cards.length)];
    setMessage(`${players[currentPlayerIndex].name} - ${card}`);
    
    const updated = [...players];
    if (card.includes('احصل')) {
      const amount = parseInt(card.match(/\d+/)[0]);
      updated[currentPlayerIndex].money += amount;
    } else if (card.includes('ادفع')) {
      const amount = parseInt(card.match(/\d+/)[0]);
      updated[currentPlayerIndex].money -= amount;
    } else if (card.includes('السجن') && !card.includes('اخرج')) {
      updated[currentPlayerIndex].position = 10;
      updated[currentPlayerIndex].inJail = true;
    } else if (card.includes('البداية')) {
      updated[currentPlayerIndex].position = 0;
      updated[currentPlayerIndex].money += 200;
    }
    
    setPlayers(updated);
    setTimeout(() => {
      if (dice1 !== dice2) nextPlayer();
      else setMessage(`${updated[currentPlayerIndex].name} - العب مرة أخرى!`);
    }, 3000);
  };

  const nextPlayer = () => {
    setDoubles(0);
    let nextIndex = (currentPlayerIndex + 1) % numPlayers;
    while (players[nextIndex].bankrupt) {
      nextIndex = (nextIndex + 1) % numPlayers;
      if (nextIndex === currentPlayerIndex) break;
    }
    setCurrentPlayerIndex(nextIndex);
    setMessage(`${players[nextIndex].name} - دورك!`);
  };

  const getBoardPosition = (index) => {
    const positions = [
      // Bottom row (0-10)
      { bottom: '0', right: '0', width: '80px', height: '80px' },
      { bottom: '0', right: '80px', width: '60px', height: '80px' },
      { bottom: '0', right: '140px', width: '60px', height: '80px' },
      { bottom: '0', right: '200px', width: '60px', height: '80px' },
      { bottom: '0', right: '260px', width: '60px', height: '80px' },
      { bottom: '0', right: '320px', width: '60px', height: '80px' },
      { bottom: '0', right: '380px', width: '60px', height: '80px' },
      { bottom: '0', right: '440px', width: '60px', height: '80px' },
      { bottom: '0', right: '500px', width: '60px', height: '80px' },
      { bottom: '0', right: '560px', width: '60px', height: '80px' },
      { bottom: '0', right: '620px', width: '80px', height: '80px' },
      // Left side (11-19)
      { bottom: '80px', right: '620px', width: '80px', height: '60px' },
      { bottom: '140px', right: '620px', width: '80px', height: '60px' },
      { bottom: '200px', right: '620px', width: '80px', height: '60px' },
      { bottom: '260px', right: '620px', width: '80px', height: '60px' },
      { bottom: '320px', right: '620px', width: '80px', height: '60px' },
      { bottom: '380px', right: '620px', width: '80px', height: '60px' },
      { bottom: '440px', right: '620px', width: '80px', height: '60px' },
      { bottom: '500px', right: '620px', width: '80px', height: '60px' },
      { bottom: '560px', right: '620px', width: '80px', height: '60px' },
      { bottom: '620px', right: '620px', width: '80px', height: '80px' },
      // Top row (21-29)
      { bottom: '620px', right: '560px', width: '60px', height: '80px' },
      { bottom: '620px', right: '500px', width: '60px', height: '80px' },
      { bottom: '620px', right: '440px', width: '60px', height: '80px' },
      { bottom: '620px', right: '380px', width: '60px', height: '80px' },
      { bottom: '620px', right: '320px', width: '60px', height: '80px' },
      { bottom: '620px', right: '260px', width: '60px', height: '80px' },
      { bottom: '620px', right: '200px', width: '60px', height: '80px' },
      { bottom: '620px', right: '140px', width: '60px', height: '80px' },
      { bottom: '620px', right: '80px', width: '60px', height: '80px' },
      { bottom: '620px', right: '0', width: '80px', height: '80px' },
      // Right side (31-39)
      { bottom: '560px', right: '0', width: '80px', height: '60px' },
      { bottom: '500px', right: '0', width: '80px', height: '60px' },
      { bottom: '440px', right: '0', width: '80px', height: '60px' },
      { bottom: '380px', right: '0', width: '80px', height: '60px' },
      { bottom: '320px', right: '0', width: '80px', height: '60px' },
      { bottom: '260px', right: '0', width: '80px', height: '60px' },
      { bottom: '200px', right: '0', width: '80px', height: '60px' },
      { bottom: '140px', right: '0', width: '80px', height: '60px' },
      { bottom: '80px', right: '0', width: '80px', height: '60px' }
    ];
    
    return positions[index];
  };

  if (!gameStarted) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-green-700 via-green-600 to-emerald-700 flex items-center justify-center p-4">
        <div className="bg-white rounded-2xl shadow-2xl p-8 max-w-md w-full">
          <div className="text-center mb-8">
            <h1 className="text-4xl font-bold text-green-800 mb-2">MONOPOLY</h1>
            <p className="text-gray-600">مونوبولي - لعبة العقارات</p>
          </div>
          
          <div className="space-y-6">
            <div>
              <label className="block text-gray-700 font-semibold mb-2 flex items-center gap-2">
                <Users size={20} />
                عدد اللاعبين
              </label>
              <select 
                value={numPlayers} 
                onChange={(e) => setNumPlayers(Number(e.target.value))}
                className="w-full border-2 border-gray-300 rounded-lg p-3 text-lg focus:border-green-500 focus:outline-none"
              >
                <option value={2}>2 لاعبين</option>
                <option value={3}>3 لاعبين</option>
                <option value={4}>4 لاعبين</option>
              </select>
            </div>
            
            <div>
              <label className="block text-gray-700 font-semibold mb-2 flex items-center gap-2">
                <DollarSign size={20} />
                المال الابتدائي
              </label>
              <input 
                type="number" 
                value={startingMoney}
                onChange={(e) => setStartingMoney(Number(e.target.value))}
                className="w-full border-2 border-gray-300 rounded-lg p-3 text-lg focus:border-green-500 focus:outline-none"
                min="500"
                step="100"
              />
            </div>
            
            <button 
              onClick={initGame}
              className="w-full bg-gradient-to-r from-green-600 to-emerald-600 text-white py-4 rounded-lg text-xl font-bold hover:from-green-700 hover:to-emerald-700 transition-all transform hover:scale-105 shadow-lg"
            >
              ابدأ اللعبة
            </button>
          </div>
        </div>
      </div>
    );
  }

  return (
    <div className="min-h-screen bg-gradient-to-br from-green-700 via-green-600 to-emerald-700 p-4">
      <div className="max-w-7xl mx-auto">
        {/* Header */}
        <div className="bg-white rounded-xl shadow-lg p-4 mb-4 flex justify-between items-center">
          <div className="flex items-center gap-4">
            <h1 className="text-3xl font-bold text-green-800">MONOPOLY</h1>
            <button 
              onClick={() => setShowSettings(!showSettings)}
              className="p-2 hover:bg-gray-100 rounded-lg transition-colors"
            >
              <Settings size={24} />
            </button>
          </div>
          
          <div className="text-center bg-yellow-100 px-6 py-3 rounded-lg border-2 border-yellow-400">
            <p className="text-sm text-gray-600">دور اللاعب</p>
            <p className="text-xl font-bold" style={{color: players[currentPlayerIndex]?.color}}>
              {players[currentPlayerIndex]?.name}
            </p>
          </div>
        </div>

        <div className="grid grid-cols-1 lg:grid-cols-4 gap-4">
          {/* Players Info */}
          <div className="lg:col-span-1 space-y-3">
            {players.map((player) => (
              <div 
                key={player.id}
                className={`bg-white rounded-xl p-4 shadow-lg border-4 ${
                  currentPlayerIndex === player.id ? 'border-yellow-400' : 'border-transparent'
                } ${player.bankrupt ? 'opacity-50' : ''}`}
              >
                <div className="flex items-center gap-3 mb-3">
                  <div 
                    className="w-8 h-8 rounded-full"
                    style={{backgroundColor: player.color}}
                  />
                  <div className="flex-1">
                    <p className="font-bold text-lg">{player.name}</p>
                    {player.bankrupt && <p className="text-red-600 text-sm font-semibold">مفلس</p>}
                    {player.inJail && <p className="text-orange-600 text-sm font-semibold">في السجن</p>}
                  </div>
                </div>
                
                <div className="space-y-2">
                  <div className="flex justify-between items-center bg-green-100 p-2 rounded">
                    <span className="text-sm font-semibold">المال:</span>
                    <span className="text-lg font-bold text-green-700">${player.money}</span>
                  </div>
                  <div className="flex justify-between items-center bg-blue-100 p-2 rounded">
                    <span className="text-sm font-semibold">العقارات:</span>
                    <span className="text-lg font-bold text-blue-700">{player.properties.length}</span>
                  </div>
                </div>
              </div>
            ))}
          </div>

          {/* Game Board */}
          <div className="lg:col-span-2">
            <div className="bg-green-50 rounded-xl shadow-2xl p-8">
              <div className="relative" style={{width: '700px', height: '700px', margin: '0 auto'}}>
                {/* Board background */}
                <div className="absolute inset-0 bg-gradient-to-br from-teal-100 to-cyan-100" style={{
                  left: '80px',
                  right: '80px',
                  top: '80px',
                  bottom: '80px',
                  borderRadius: '20px'
                }}>
                  <div className="absolute inset-0 flex items-center justify-center">
                    <div className="text-center">
                      <h2 className="text-4xl font-bold text-gray-700 mb-4">MONOPOLY</h2>
                      <div className="bg-white rounded-lg p-6 shadow-lg max-w-sm">
                        <p className="text-lg font-semibold text-gray-800 mb-3">{message}</p>
                        
                        <div className="flex gap-3 justify-center mb-4">
                          <div className="bg-red-500 text-white w-16 h-16 rounded-lg flex items-center justify-center text-3xl font-bold shadow-lg">
                            {dice1}
                          </div>
                          <div className="bg-red-500 text-white w-16 h-16 rounded-lg flex items-center justify-center text-3xl font-bold shadow-lg">
                            {dice2}
                          </div>
                        </div>
                        
                        <div className="space-y-2">
                          <button 
                            onClick={rollDice}
                            className="w-full bg-gradient-to-r from-blue-500 to-blue-600 text-white py-3 rounded-lg font-bold hover:from-blue-600 hover:to-blue-700 transition-all transform hover:scale-105 shadow-md flex items-center justify-center gap-2"
                          >
                            <Dices size={20} />
                            ارمِ النرد
                          </button>
                          
                          {properties[players[currentPlayerIndex]?.position]?.price && 
                           !players.find(p => p.properties.includes(players[currentPlayerIndex]?.position)) && (
                            <button 
                              onClick={buyProperty}
                              className="w-full bg-gradient-to-r from-green-500 to-emerald-600 text-white py-3 rounded-lg font-bold hover:from-green-600 hover:to-emerald-700 transition-all transform hover:scale-105 shadow-md flex items-center justify-center gap-2"
                            >
                              <Building2 size={20} />
                              اشترِ
                            </button>
                          )}
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

                {/* Board Spaces */}
                {properties.map((prop, idx) => {
                  const pos = getBoardPosition(idx);
                  const playersHere = players.filter(p => p.position === idx && !p.bankrupt);
                  const owner = players.find(p => p.properties.includes(prop.id));
                  
                  return (
                    <div
                      key={idx}
                      className="absolute border-2 border-gray-800 bg-white overflow-hidden"
                      style={{
                        ...pos,
                        boxShadow: '0 2px 4px rgba(0,0,0,0.2)'
                      }}
                    >
                      {/* Property color bar */}
                      {prop.type === 'property' && (
                        <div 
                          className="h-5"
                          style={{backgroundColor: prop.color}}
                        />
                      )}
                      
                      {/* Property icon and name */}
                      <div className="p-1 text-center flex flex-col items-center justify-center h-full">
                        {prop.type === 'go' && <Home size={16} className="text-red-600 mb-1" />}
                        {prop.type === 'property' && <Building2 size={14} className="mb-1" />}
                        {prop.type === 'station' && <Train size={14} className="mb-1" />}
                        {prop.type === 'utility' && (prop.name.includes('كهرباء') ? <Zap size={14} className="mb-1" /> : <Droplet size={14} className="mb-1" />)}
                        {prop.type === 'tax' && <DollarSign size={14} className="text-pink-600 mb-1" />}
                        {prop.type === 'chance' && <HelpCircle size={14} className="text-orange-600 mb-1" />}
                        {prop.type === 'community' && <HelpCircle size={14} className="text-blue-600 mb-1" />}
                        {prop.type === 'jail' && <span className="text-xs font-bold mb-1">🔒</span>}
                        {prop.type === 'gotojail' && <span className="text-xs font-bold mb-1">👮</span>}
                        {prop.type === 'parking' && <span className="text-xs font-bold mb-1">🅿️</span>}
                        
                        <p className="text-xs font-bold leading-tight" style={{fontSize: '9px'}}>
                          {prop.name}
                        </p>
                        
                        {prop.price && (
                          <p className="text-xs font-semibold text-green-700" style={{fontSize: '8px'}}>
                            ${prop.price}
                          </p>
                        )}
                        
                        {/* Owner indicator */}
                        {owner && (
                          <div 
                            className="w-3 h-3 rounded-full mt-1"
                            style={{backgroundColor: owner.color}}
                          />
                        )}
                        
                        {/* Players on this space */}
                        {playersHere.length > 0 && (
                          <div className="flex gap-1 mt-1 flex-wrap justify-center">
                            {playersHere.map((p) => (
                              <div
                                key={p.id}
                                className="w-3 h-3 rounded-full border-2 border-white"
                                style={{backgroundColor: p.color}}
                              />
                            ))}
                          </div>
                        )}
                      </div>
                    </div>
                  );
                })}
              </div>
            </div>
          </div>

          {/* Game Info */}
          <div className="lg:col-span-1 space-y-3">
            <div className="bg-white rounded-xl p-4 shadow-lg">
              <h3 className="font-bold text-lg mb-3 flex items-center gap-2">
                <Building2 size={20} />
                قواعد اللعبة
              </h3>
              <div className="space-y-2 text-sm text-gray-700">
                <p>• ارمِ النرد للتحرك</p>
                <p>• اشترِ العقارات لكسب الإيجار</p>
                <p>• المرور من البداية: +200$</p>
                <p>• نرد متطابق: العب مرة أخرى</p>
                <p>• 3 أنراد متطابقة: اذهب للسجن</p>
                <p>• السجن: 3 محاولات أو ادفع 50$</p>
                <p>• الفوز: آخر لاعب غير مفلس</p>
              </div>
            </div>

            <div className="bg-white rounded-xl p-4 shadow-lg">
              <h3 className="font-bold text-lg mb-3">ألوان العقارات</h3>
              <div className="space-y-2 text-xs">
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'brown'}}></div>
                  <span>بني - رخيص</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'lightblue'}}></div>
                  <span>أزرق فاتح</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'purple'}}></div>
                  <span>بنفسجي</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'orange'}}></div>
                  <span>برتقالي</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'red'}}></div>
                  <span>أحمر</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'yellow'}}></div>
                  <span>أصفر</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'green'}}></div>
                  <span>أخضر</span>
                </div>
                <div className="flex items-center gap-2">
                  <div className="w-6 h-6 rounded" style={{backgroundColor: 'blue'}}></div>
                  <span>أزرق - غالي</span>
                </div>
              </div>
            </div>

            <button 
              onClick={() => {
                setGameStarted(false);
                setPlayers([]);
                setCurrentPlayerIndex(0);
                setMessage('');
              }}
              className="w-full bg-red-500 text-white py-3 rounded-lg font-bold hover:bg-red-600 transition-all shadow-md"
            >
              إنهاء اللعبة
            </button>
          </div>
        </div>
      </div>
    </div>
  );
};

export default MonopolyGame;
